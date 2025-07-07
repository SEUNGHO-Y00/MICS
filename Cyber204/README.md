# CYBER 204: Software Security

## 1. Software Security Overview

1. Introduction
* Software Security Landscape
* Cost of Security Vulnerabilities

2. Security Flaws and Causes
* The raange of security flaws
* Causes of insecure software

3. Secure Program Design
* Secure Design Principles

4. First Look at Vulnerabilities
* Classifying and Recording Vulnerabilities
* Some Representative Exploits
* Detecting and Reporting Vulnerabilities

## 2. Input Validation

1. Overview
* Basic Principles

2. Input Validation Practice
* Robust Input Handling
* Regular Expressions for Input Validation
* Handling File Names
* Character Encoding Issues

3. Command Injection
* Command Injection: Overview
* Command Injection: Language Specifics
* Protection Against Command Injection

## 3. Web Application Security, Part 1

1. Web Security Overview
* OWASP Top 10 Vulnerabilities
* Cross Domain Interaction

2. SQL Injection
* SQL Injection Basics
* Flavors of SQL Injection
* Securing Against SQL Injection

3. Cross-Site Scripting
* Reflected and Stored XSS
* Protections Against XSS

## 4. Web Application Security, Part 2

1. Other Scripting Attacks
* Cross-Site Script Inclusion
* Heap Spraying

2. Cross-Site Request Forgery
* Cross-Site Request Forgery
* CSRF Prevention

3. Other Unintended Execution Attacks
* Clickjacking
* Workflow and Authentication Attacks -3

4. Sandboxing
* Sandboxing: Solutions and Limitations

## 5. Object-orientation and Concurrency

1. Object-Oriented Specifics
* Object-Oriented Specifics
* Constructors and Destructors-2
* Containeers
* Copying Issues

2. Exception Handling
* Exception Handling

3. Concurrency Issues
* Locking
* Visibility and Atomicity
* Race Conditions

## 6. Secure Program Design

1. Principles of Secure Program Design
* Secure Design: Overview
* Minimize Privilege
* Avoid Race Conditions

2. Environment and Configuration
* Configuration and Initialization
* Secure Environment

3. Secure Interactions
* Secure Interfacing
* Secure Library Usage

## 7. Secure Program Design

1. Information Flow
* Output Information Judiciously
* Information Flow Foundations
* Side Channels
* Meltdown and Spectre

2. File System Issues
* Files: Unix Specifics
* Files: Windows Specifics

3. Process Management
* Processes: Unix Specifics
* Processes: Windows Specifics

## 8. Memory Corruption Vulnerabilities

1. Introduction to Buffer Overflows
* Introduction to Memory Vulnerabilities
* Classic Buffer Overflow in C

2. How Buffer Overflows Happen
* How Buffer Overflows Happen

3. Program Execution
* Program Execution. Calling Conventions

4. Input Vulnerabilities
* Insecure Program Input

5. Prevention and Protection
* Why Are Buffer Overflows So Frequent?
* Memory Protections

## 9. Advanced Memory Corruption Attacks and Defenses

1. Variants Memory Overflow
* Variants of Memory Corruption
* Integer Overflow/Wraparound

2. Heap Overflows and Pointer Overwrites
* Heap Overflows
* Pointer Overwrites

3. Examples of Pointer Vulnerabilities
* Examples of Pointer Vulnerabilities - Demo

4. Misusing Existing Code
* Return-into-libc Attack
* Return-Oriented Programming

5. Advanced Memory Protections
* Attacks and Protections Overview
* Control Flow Integrity

## 10. Using Cryptographic APIs

1. Passwords are Authentication
* Password Guidelines
* Authentication Logic

2. Randomness
* Secure Random Numer Generator
* Predictability Flaws

3. Improper Cryptography Use
* Weak Hash Functions
* Improper Encryption
* Protocol and Design Flaws

## 11. Mobile Application Security

1. Mobile Security Overview
* Major Security Issues
* Android Application Design

2. Application Permissions
* Android Application Permissions
* Permission Attacks

3. Internal Security Issues
* "Your phone is a mini-internet!"
* Dynamic Loading and Native Code

4. Securing Applications
* Secure Applications
* Detecting Malicious Apps and Activity

## 12. Security Analysis

1. Static Analysis
* Principles and Targeted Errors
* Using Static Analysis Tools

2. Dynamic Analysis
* Code Instrumentation
* Taint Analysis
* Symbolic Execution
* Sanitization Libraries

3. Formal Methods
* Scope of Formal Verification
* Using Verification in Practice

## 13. Security Testing

1. Security Testing Landscape
* Security Testing Overview
* Vulnerability Scanning
* Penetration Testing

2. Fuzz Testing
* Fuzzing Programs
* Fuzzing Web Applications

3. Model-Based Testing
* Using Models in Testing
* Model Learning

4. Approaching the Testing Process
* Selecting Testing Techniques

## 14. Managing Software Security

1. Security Models
* Introduction to Security Engineering
* Building Security in Maturity Model

2. Managing Secure Development
* Organizational Issues
* Requirement Engineering
* Secure Design Issues
* Risk Management

3. Security Evaluation and Assurance
* Security Assurance
* Security Evaluation. Common Criteria

