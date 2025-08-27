### 🔹 Exercise 2 — Create & Run a Script  
👉 Goal: Learn how to create and execute a simple shell script.  

#### 📝 Steps  
```bash
touch script.sh
echo "echo 'Hello, I am running as a script!'" >> script.sh
ls -l script.sh
chmod +x script.sh
./script.sh
```

#### 📘 What I Learned  
- `ls -l` → Check file permissions  
- `chmod +x` → Make a file executable  
- `./script.sh` → Run a shell script  

#### 💡 Output  
```text
Hello, I am running as a script!
```

#### 📌 Key Takeaways  
- Linux treats **everything as a file** (even scripts and devices)  
- File permissions (`rwx`) define who can **read, write, execute**  
- Small scripts = first step to **automation in DevOps**  
