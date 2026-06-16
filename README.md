# Project 41: AWS S3 Cross-Region Replication (Disaster Recovery Setup)

## 📌 Project Overview
This project demonstrates how to set up an automated, production-ready Disaster Recovery (DR) solution using Amazon S3 Cross-Region Replication (CRR). The goal is to ensure high availability and data redundancy across geographically separated AWS regions.

## 🛠️ Architecture Details
* **Source Bucket:** `azam-architect-primary-41` (Region: US East - N. Virginia)
* **Destination Bucket:** `azam-architect-backup-41` (Region: Asia Pacific - Mumbai)

## 🚀 Key Steps Implemented
1. **Multi-Region Setup:** Created S3 buckets in two distinct AWS regions (US and India).
2. **Bucket Versioning:** Enabled Versioning on both source and destination buckets (a strict prerequisite for replication).
3. **IAM Security:** Configured a secure IAM Role with necessary permissions to allow S3 to replicate objects automatically.
4. **Replication Rule:** Created a custom replication rule (`Sync-To-Mumbai`) to sync all new objects in real-time.
5. **Live DR Testing:** Uploaded sample data to the US bucket and verified automated, near-instantaneous replication to the Mumbai bucket.
