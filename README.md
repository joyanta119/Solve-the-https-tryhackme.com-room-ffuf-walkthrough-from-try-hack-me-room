# Solve-the-https-tryhackme.com-room-ffuf-walkthrough-from-try-hack-me-room
My walkthrough and notes from the TryHackMe FFUF room, covering web enumeration, directory discovery, parameter fuzzing, and filtering techniques.
# TryHackMe - FFUF

## 📌 Project Overview

This repository contains my notes, learning experience, and practical work from completing the **FFUF room on TryHackMe**.

FFUF (Fuzz Faster U Fool) is a web fuzzing tool used for discovering hidden directories, files, parameters, virtual hosts, and other resources within web applications.

Through this room, I practiced different fuzzing and web enumeration techniques using FFUF.

---

## 🎯 Learning Objectives

The main objective of this lab was to understand how web fuzzing works and how FFUF can be used for reconnaissance and enumeration.

During this lab, I practiced:

- Directory discovery
- File discovery
- Web content enumeration
- Parameter fuzzing
- Subdomain and virtual host discovery
- Response filtering
- Response matching
- Using custom wordlists
- Identifying hidden web resources

---

## 🛠️ Tools Used

- TryHackMe
- FFUF
- Linux
- Web Browser
- Terminal

---

## 🌐 Lab Platform

This practical lab was completed on TryHackMe.

🔗 Room Link: https://tryhackme.com/room/ffuf

---

# 🔍 What is FFUF?

FFUF stands for **Fuzz Faster U Fool**.

It is a fast web fuzzing tool that can be used to discover hidden resources and perform web enumeration.

FFUF allows users to send multiple requests using wordlists and identify valid responses based on factors such as:

- HTTP status codes
- Response size
- Number of words
- Number of lines
- Response time

It is commonly used during the reconnaissance and enumeration phases of web application security testing.

---

# 📂 Directory Fuzzing

One of the main uses of FFUF is discovering hidden directories and files on a web server.

A typical command structure is:

```bash
ffuf -w wordlist.txt -u http://TARGET/FUZZ
