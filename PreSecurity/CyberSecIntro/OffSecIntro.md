---
title: Hacking Your First Machine – Writeup
layout: default
---

# 🧠 Hacking Your First Machine – TryHackMe Writeup

## 🛠️ Step 1: Initial Enumeration with Gobuster

Open a terminal and run `gobuster` to enumerate potential hidden directories on the **FakeBank** website.

We’ll use the following command:

```bash
gobuster dir -u http://fakebank.thm -w wordlist.txt
```

**Explanation:**
- `-u`: The target URL to scan  
- `-w`: Path to the wordlist (a list of common directory/file names)

> 📝 This will brute-force potential directories or files by appending each word in the wordlist to the base URL.

---

## 🔍 Step 2: Reviewing the Results

The scan should return a few interesting paths:

- `/images`
- `/bank-transfer`

Let’s check them out one by one.

### 🔸 `/images`
Nothing particularly interesting here.

### 🔹 `/bank-transfer`
**This is where the action is.** It takes us to an **internal staff admin portal** for initiating bank transfers. Definitely a high-value target.

---

## 💸 Step 3: Exploiting the Functionality

Let’s try to initiate a transfer of `$2000` from account `2276` to our own account `8881`.

Once the transaction is submitted, **TryHackMe should display the flag** — confirming successful exploitation.

---

## 🧾 Notes & Tips

- `gobuster` is a powerful directory brute-forcing tool.
- You can view more flags by running:
  ```bash
  man gobuster
  ```
  or
  ```bash
  gobuster -h
  ```

### ⚙️ Other useful flags:
- `-x`: Specify file extensions (e.g., `.php`, `.html`)
- `-t`: Set number of threads for faster scanning
- `-o`: Output results to a file

---

## ✅ Outcome

- Learned basic directory brute-forcing
- Found and exploited a vulnerable internal banking portal
- Captured the flag 🏁
