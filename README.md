# CS-405-Secure-Coding-Portfolio

## Overview

This portfolio demonstrates my application of secure software development principles using C and C++. The included projects explore common software vulnerabilities, methods for reducing security risk, automated testing, static code analysis, encryption, and security policy development.

The work reflects a security-first approach in which vulnerabilities are considered throughout design, implementation, testing, and maintenance. Each artifact demonstrates a different part of the secure software development lifecycle.

## Core Competencies

- Secure C and C++ development
- Input validation and numeric range checking
- Buffer overflow prevention
- SQL injection mitigation
- Memory-safe resource management
- Structured exception handling
- Positive and negative unit testing
- Static code analysis
- Threat identification and prioritization
- Security policy development
- DevSecOps and shift-left security
- Authentication, authorization, and auditing
- Encryption and data protection
- Defense-in-depth planning

## Technologies and Tools

- C and C++
- Microsoft Visual Studio
- Google Test
- Cppcheck
- SQLite
- Git and GitHub
- Microsoft PowerPoint

## Portfolio Artifacts

### Security Policy

The GreenPace security policy defines coding standards, security principles, threat levels, recommended automation tools, encryption requirements, and Triple-A controls. It demonstrates how security expectations can be documented clearly and applied consistently by development teams.

The policy addresses:

- Data types and numeric values
- String correctness
- SQL injection prevention
- Memory protection
- Assertions
- Exception handling
- File path validation
- Polymorphic object destruction
- Thread synchronization
- Encryption at rest, in transit, and in use
- Authentication, authorization, and auditing
- DevSecOps automation

### Security Policy Presentation

The presentation explains the security policy, threat-prioritization process, secure coding standards, unit-testing strategy, automation recommendations, and defense-in-depth approach.

[Watch the GreenPace Security Policy Presentation](https://www.youtube.com/watch?v=v9mYnESzbz0)

### Secure Coding Projects

#### Numeric Overflow Prevention

Demonstrates how numeric overflow and underflow can occur across multiple C++ data types. The implementation uses range validation and boundary checking to identify unsafe operations before they produce incorrect results or undefined behavior.

#### Buffer Overflow Prevention

Demonstrates the risks created by writing beyond allocated memory boundaries. The corrected implementation validates input size and applies safer data-handling practices to prevent memory corruption.

#### SQL Injection Prevention

Demonstrates how untrusted input can alter dynamically constructed SQL statements. The secure implementation uses prepared statements and parameter binding to separate executable SQL from user-supplied data.

#### Exception Handling

Implements standard exceptions, a custom exception class, specific catch handlers, and a catch-all handler. The project demonstrates how structured exception handling can prevent abrupt termination while providing useful error information.

#### Vector Unit Testing

Uses the Google Test framework to evaluate `std::vector` behavior through positive and negative tests. The test suite verifies collection creation, insertion, resizing, capacity, clearing, erasing, reservation, and out-of-range exception handling.

#### File Encryption

Implements character-by-character XOR transformation, text-file loading, and file-output operations. The activity demonstrates the reversible nature of XOR and the importance of accounting for key length.

XOR is used here for educational purposes and would not be appropriate as a replacement for modern production encryption standards.

#### Static Code Analysis

Uses Cppcheck and Visual Studio analysis to identify defects such as unsafe array access, infinite recursion, invalid iterator use, dangling pointers, ineffective assertions, and misleading control flow.

The comparison demonstrates the value of combining multiple analysis tools because individual tools may detect different categories of issues.

## Security Approach

My approach begins by treating all external data as untrusted. Input must be validated before it affects application state, database queries, memory operations, or resource access. Security controls should be layered so that the failure of one control does not expose the entire system.

I prioritize vulnerabilities according to their potential impact, likelihood of exploitation, remediation cost, and effect on confidentiality, integrity, and availability. High-impact vulnerabilities involving memory corruption, injection, unauthorized access, or sensitive data exposure receive the highest remediation priority.

Automated unit tests and static analysis should be incorporated into the development pipeline so defects can be identified close to their source. This shift-left approach reduces remediation costs and helps teams enforce coding standards consistently.

## What I Learned

Developing these artifacts strengthened my understanding that secure coding is not a separate task performed after development. It is a continuous responsibility that begins during architecture and continues through implementation, testing, deployment, and maintenance.

The most important lessons from this work include:

- Validate data before trusting or processing it.
- Prefer memory-safe resource-management techniques.
- Use parameterized database operations instead of query concatenation.
- Catch specific exceptions whenever possible.
- Test both expected behavior and failure conditions.
- Use automated tools to supplement manual review.
- Apply least privilege and defense in depth.
- Document security requirements so other developers can reproduce them.
- Treat security policies as enforceable engineering standards.

## Repository Contents

This repository contains:

- The GreenPace security policy
- A link to the recorded security policy presentation
- Numeric overflow source code
- Buffer overflow source code
- SQL injection source code
- Exception-handling source code
- Google Test unit-testing source code
- Encryption source code and supporting data files
- Static-analysis materials
- A portfolio reflection

Generated Visual Studio build directories and environment-specific cache files have been excluded to keep the repository focused on source code and relevant documentation.

## Professional Value

This portfolio demonstrates my ability to evaluate software from both development and security perspectives. I can identify vulnerabilities, explain their risks, implement safer alternatives, test expected and unexpected behavior, use automated analysis tools, and communicate security recommendations to technical and nontechnical stakeholders.

These skills support work in application development, secure software engineering, quality assurance, DevSecOps, and full-stack development.

## Author

**Deanna Talton**

Computer Science Student and Software Developer

[GitHub Profile](https://github.com/Deanna-Talton)
