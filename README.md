
# Distributed File Backup System

## 📌 Project Overview
This project implements a **Distributed File Backup System** that replicates files across multiple nodes to ensure **data redundancy** and **fault tolerance**. When a file is uploaded, it is backed up to several nodes in the network to protect against data loss due to hardware failures or network issues.

## 🎯 Key Features
- File replication across multiple storage nodes  
- Redundant storage to ensure high availability  
- Fault-tolerant file access  
- Simple CLI or API interface for uploading and retrieving files  
- Logging and error handling for node failures  

## 🏗️ System Architecture
- **Client**: Uploads and retrieves files.  
- **Nodes (Servers)**: Store replicated copies of files.  
- **Master Controller** (optional): Manages file distribution and replication logic.

## 🧠 Technologies Used
- Python  
- Socket Programming / gRPC  
- Threading / Multiprocessing  
- JSON / Pickle for metadata tracking  
- (Optional) Flask or FastAPI for a REST interface  

## 🛠️ How It Works
1. User uploads a file via CLI or API.
2. File is split (optional) and replicated to multiple nodes.
3. Metadata is stored for tracking replicas.
4. On retrieval, the system fetches the file from the first available node.

## 🚀 Getting Started

### Prerequisites
- Python 3.x  
- Install dependencies:
  ```bash
  pip install -r requirements.txt

## Future Enhancements
Web-based dashboard to monitor nodes and backups

File versioning support

Encryption for secure backups

Dynamic node discovery and load balancing
