# VulnLocAI: Lightweight Java Vulnerability Detection with Fine-Tuned Domain Specific Large Language Models

[![Dataset](https://img.shields.io/badge/Dataset-5054%20samples-blue)](#)
[![CWE Coverage](https://img.shields.io/badge/CWE%20Types-32-green)](#)
[![Paper](https://img.shields.io/badge/Paper-Available-red)](#)

This repository contains the **Benchmark dataset** for the evaluation framework presented in our paper: 

**"VulnLocAI: Lightweight Java Vulnerability Detection with Fine-Tuned Domain Specific Large Language Models"**

* Wala Alnozami, Obieda Ananbeh, Dae-Kyoo Kim*  
*Department of Computer Science & Engineering, Oakland University*

## 🗃️ Benchmark Overview

The Benchmark dataset provides a balanced, high-quality collection of Java vulnerability examples for research purposes:

### Dataset Statistics
- **Total Samples**: 5,054 (balanced dataset)
  - **Vulnerable**: 2,527 instances
  - **Benign**: 2,527 instances
- **Projects**: 20 real-world Java projects
- **CWE Categories**: 32 different vulnerability types
- **Programming Language**: Java

### Project Coverage
Our benchmark includes diverse Java projects from various domains:

| Domain | Examples |
|--------|----------|
| **Web Frameworks** | Apache CXF, Undertow, Vert.x |
| **Big Data** | Apache Flink, Apache Hadoop, Apache Hive |
| **Developer Tools** | OpenRefine, FitNesse |
| **Identity & Access** | Keycloak |
| **Databases** | HyperSQL, OpenTSDB, Infinispan |
| **Communication** | OpenMeetings, Wire-AVS |

#### Detailed Project Information
The following table provides comprehensive details about all 20 evaluated projects, including their associated CVEs, descriptions, and affected versions:

| **Project Name** | **CVE-ID** | **Description** | **Affected Versions** |
|------------------|------------|-----------------|----------------------|
| **eclipse-vertx** | CVE-2019-17640 | Vert.x core offers low-level, event-driven, non-blocking functionalities like HTTP, TCP, and file system access for building reactive applications. | >= 3.0.0, < 3.9.4 |
| **Apache Flink** | CVE-2020-17518 | Apache Flink is an open-source framework for real-time stream and batch data processing. | >= 1.5.1, < 1.11.3 |
| **OpenTSDB** | CVE-2020-35476 | OpenTSDB is a distributed time series database built on HBase, designed for storing and serving large-scale metrics. | <= 2.4.0 |
| **Apache Hadoop** | CVE-2022-25168 | Apache Hadoop enables distributed processing of large data sets across clusters using the MapReduce programming model and HDFS for storage. | >= 2.0.0, < 2.10.2, >= 3.0.0-alpha, < 3.2.4, >= 3.3.0, < 3.3.3 |
| **Netty** | CVE-2022-41915 | Netty is a Java-based asynchronous event-driven network application framework for rapid development of high-performance protocol servers and clients. | >= 4.1.83.Final, < 4.1.86.Final |
| **Undertow** | CVE-2018-1067 | Undertow is a flexible Java web server offering blocking and non-blocking APIs, enabling composable architectures and full servlet 4.0 support. | <= 7.1.1.GA |
| **wire-avs** | CVE-2021-41193 | Wire is a secure messaging platform; this CVE relates to its use of pre-built Google WebRTC binaries in AVS. | <= 7.1.1.GA |
| **Apache Dubbo** | CVE-2021-36161 | Apache Dubbo is a high-performance Java-based RPC framework offering microservices communication and service governance. | < 7.1.12 |
| **Apache NiFi** | CVE-2018-17195 | Apache NiFi automates data flow between systems, providing a user-friendly interface for data ingestion, routing, and transformation. | < 2.7.13 |
| **James** | CVE-2022-45935 | Apache James is a modular Java-based mail server platform, allowing custom email solutions with extensible components. | >= 1.0.0, <= 1.7.1 |
| **Infinispan** | CVE-2019-10174 | Infinispan is an open-source in-memory key/value data store and cache, offering high availability and scalability. | <= 8.2.11.Final, >= 9.0.0.Final, <= 9.4.16.Final |
| **HyperSQL** | CVE-2022-41853 | HyperSQL Database (HSQLDB) is a relational database management system written in Java, offering in-memory and disk-based tables. | < 2.7.1 |
| **Apache Hive** | CVE-2022-41137 | Apache Hive provides SQL-like querying for large datasets stored in Hadoop, facilitating data warehousing and analysis. | 4.0.0-alpha-1 |
| **Openmeetings** | CVE-2024-54676 | OpenMeetings is an Apache-licensed platform for video conferencing, instant messaging, and collaborative document editing. | >= 2.1.0, < 8.0.0 |
| **Eclipse GlassFish** | CVE-2024-9329 | Eclipse GlassFish is a Jakarta EE-compliant application server, offering implementations of all Jakarta EE APIs. | >= 2.1.0, < 8.0.0 |
| **Keycloak** | CVE-2024-8883 | Keycloak is an open-source identity and access management solution, supporting single sign-on with OAuth2, OpenID Connect, and SAML. | < 7.0.17 |
| **Hugegraph-toolchain** | CVE-2024-27347 | HugeGraph-Toolchain integrates utilities for HugeGraph, including over five main modules for enhanced graph data management. | <= 22.0.12, >= 23.0.0, <= 24.0.7, >= 25.0.0, <= 25.0.5 |
| **Apache CXF** | CVE-2024-28752 | Apache CXF is an open-source services framework facilitating the development of SOAP and RESTful web services. | >= 1.0.0, < 1.3.0 |
| **FitNesse** | CVE-2024-39610 | FitNesse is a web server-based tool for specifying and verifying application acceptance criteria through collaborative testing. | < 3.5.8, >= 3.6.0, < 3.6.3, >= 4.0.0, < 4.0.4 |
| **OpenRefine** | CVE-2024-47882 | OpenRefine is a Java-based tool for cleaning and transforming messy data, enhancing data quality and consistency. | < 3.8.0 |

### CWE Distribution
The dataset covers 32 CWE types ranging from highly prevalent to rare vulnerabilities. Below is the complete distribution of all CWE categories in our benchmark:

| **CWE-ID** | **Count** | **CWE-ID** | **Count** | **CWE-ID** | **Count** | **CWE-ID** | **Count** |
|------------|-----------|------------|-----------|------------|-----------|------------|-----------|
| **CWE-798** | **632** | **CWE-400** | **58** | **CWE-942** | **18** | **CWE-280** | **3** |
| **CWE-23** | **280** | **CWE-1004** | **52** | **CWE-208** | **18** | **CWE-330** | **2** |
| **CWE-319** | **216** | **CWE-547** | **52** | **CWE-326** | **14** | **CWE-613** | **1** |
| **CWE-918** | **201** | **CWE-78** | **49** | **CWE-502** | **11** | **CWE-200** | **1** |
| **CWE-79** | **168** | **CWE-295** | **48** | **CWE-134** | **8** | **CWE-297** | **1** |
| **CWE-113** | **149** | **CWE-614** | **46** | **CWE-327** | **8** | **CWE-114** | **1** |
| **CWE-611** | **121** | **CWE-352** | **31** | **CWE-90** | **8** | **CWE-347** | **1** |
| **CWE-470** | **93** | **CWE-209** | **29** | **CWE-501** | **7** | | |
| **CWE-601** | **75** | **CWE-89** | **29** | **CWE-256** | **3** | | |
| **CWE-916** | **68** | **CWE-732** | **22** | **CWE-074** | **3** | | |

