# linux-devops-journey
"Hands-on linux practice repo documenting my learn in public journey into devops and cloud computiing."
# 🐧 Linux Practice – Day 1  
> My first step in mastering Linux for **DevOps + Cloud Computing** 🚀 

![Linux Banner](https://img.shields.io/badge/Linux-DevOps-blue?style=for-the-badge&logo=linux&logoColor=white)  
![Status](https://img.shields.io/badge/Status-Completed-green?style=flat-square)  
![Learn In Public](https://img.shields.io/badge/Learn%20In%20Public-%E2%9C%94-lightgrey?style=flat-square)  

---

## 📖 Overview  
This repo documents my **first Linux hands-on exercises** where I practiced:  
- 🗂️ File management (`pwd`, `ls`, `mkdir`, `touch`, `cat`, `cp`, `mv`)  
- ⚡ Creating & executing shell scripts (`script.sh`)  
- 🔑 Understanding **permissions** with `ls -l` and `chmod`  

This is part of my **DevOps & Cloud Learn-in-Public Journey**.  

---

## 🎯 Exercises  

### 🔹 Exercise 1 — File Management  
👉 Goal: Learn basic file handling commands in Linux.  

#### 📌 Code I Practiced
```bash
# Show current directory
pwd

# List files
ls

# Create a new folder
mkdir DevOpsPractice

# Enter the folder
cd DevOpsPractice

# Create a new empty file
touch hello.txt

# Write text into the file
echo "My first Linux practice file" > hello.txt

# Read the file
cat hello.txt

# Copy the file
cp hello.txt copy.txt

# Rename/Move the file
mv copy.txt moved.txt
```
#### 📘 What I Learned  

- `pwd` → Print current directory  
- `ls` & `ls -l` → List files with permissions/owners/sizes  
- `touch` → Create empty files  
- `echo >` → Write into files  
- `cp` → Copy files  
- `mv` → Move/rename files  


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

- ---

## 🧑‍💻 Author  

👋 Hi, I’m **Rushikesh Dhumal**  
– 3rd-year **CSE student**, Cloud & DevOps enthusiast.  

🌐 [LinkedIn](https://www.linkedin.com/in/rushikesh-dhumal-613309246/)  
🐙 [GitHub](https://github.com/Rishi2911)  
📝 Documenting my **DevOps + Cloud Journey** publicly. 
