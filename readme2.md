 🐧 Linux Basics for DevOps – Day 2: Users, Permissions & Processes

If you’re starting your journey in DevOps & Cloud Computing, Linux is going to be your best friend (and sometimes your biggest challenge 😅).

On Day 2 of my Learn-in-Public journey, I explored Users, Permissions, and Processes in Linux. These are fundamental concepts every DevOps engineer must master, because managing servers means managing who can do what and what is running where.

👤 Users – Who Are You in Linux?

Linux is a multi-user system, meaning multiple people can use the same machine simultaneously. That’s why it’s important to always know which user you are logged in as.

🔹 Check your current user:

whoami


🔹 Check all logged-in users:

who


Why this matters: In real servers, you might be logged in as a normal user but need to switch to root (admin). Knowing your user context helps avoid accidental mistakes.

🔑 Permissions – Controlling Access

Every file in Linux has three layers of permissions:

User (u) → the owner of the file

Group (g) → a team of users

Others (o) → everyone else

And three types of actions:

r → read

w → write

x → execute

📌 View file permissions:

ls -l


Example output:

-rw-r--r--  1 rushi staff   20 Aug 27  hello.txt


🔹 Breakdown:

rw- → user (owner) can read & write

r-- → group can only read

r-- → others can only read

You can change permissions using chmod:

chmod +x hello.txt      # Add execute permission
chmod u-w hello.txt     # Remove write for user
chmod 777 hello.txt     # Full access for all (⚠️ dangerous!)


👉 As a DevOps engineer, you’ll use permissions daily to secure files and scripts.

⚙️ Processes – The Programs Behind the Scenes

A process is simply a running program. Linux allows you to see and manage them easily.

🔹 View running processes:

ps


🔹 View all processes in detail:

ps aux


🔹 Search for a specific process:

ps aux | grep chrome


🔹 Kill a process by PID (Process ID):

kill <PID>


👉 Replace <PID> with the number from ps aux.
This is super useful when a program hangs or eats up all your CPU.

📝 Key Takeaways

Linux is multi-user → always check which user you are.

Permissions are critical for security. Avoid chmod 777 unless absolutely necessary.

Processes are the heartbeat of your system. Knowing how to monitor & manage them is essential.

🚀 Why This Matters for DevOps

As future DevOps & Cloud engineers, we’ll work with servers running critical applications. Imagine:

If permissions are too open → hackers can exploit them.

If a runaway process isn’t killed → server crashes.

If you don’t know which user you are → one wrong command could break production.

That’s why mastering these basics early is a game-changer.
