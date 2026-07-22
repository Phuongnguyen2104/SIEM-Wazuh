# Môi trường thực nghiệm

Tài liệu này mô tả phần cứng, phần mềm, nền tảng ảo hóa và cấu hình mạng được sử dụng để triển khai dự án Giám sát An ninh mạng dựa trên SIEM sử dụng Wazuh (SIEM-Based Cybersecurity Monitoring Using Wazuh).

---
# Máy chủ

| Component               | Specification                                                     |
| ----------------------- | ----------------------------------------------------------------- |
| Hệ điều        | Windows 11 (Host)                                                 |
| Nền tảng ảo  | VMware Workstation                                                |
| Mục đích                | Lưu trữ tất cả các máy ảo được sử dụng trong phòng thí nghiệm an ninh mạng. |

---

# Máy ảo

# Máy Wazuh Server

| Component        | Configuration                                 |
| ---------------- | --------------------------------------------- |
| Hệ điều hành | Ubuntu 22.04 LTS                              |
| RAM              | 8 GB                                          |
| CPU              | 4 Cores                                       |
| Storage          | 90 GB                                         |
| Vai trò        | Wazuh Manager, Wazuh Dashboard, Wazuh Indexer |

### Các dịch vụ đã cài đặt 

- Wazuh Server
- Wazuh Dashboard
- Wazuh Indexer
- File Integrity Monitoring
- Thu thập nhật ký

## Windows 10 Endpoint
  
| Component        | Configuration      |
| ---------------- | ------------------ |
| Hệ điều hành | Windows 10 x64     |
| RAM              | 4 GB               |
| CPU              | 2 Cores            |
| Storage          | 60 GB              |
| Vai trò            | Điểm cuối được giám sát |

### Các thành phần đã cài đặt

- Wazuh Agent
- Windows Event Logs
- Windows Defender

  ---

  ## Linux Endpoint

| Component        | Configuration      |
| ---------------- | ------------------ |
| Hệ điều hành | Linux   |
| RAM              | 2 GB               |
| CPU              | 2 Cores            |
| Storage          | 40 GB              |
| Vai trò           | Điểm cuối được giám sát |

### Các thành phần đã cài đặt

- Wazuh agent
- Firewall Iptables

## Kali Linux

| Component        | Configuration             |
| ---------------- | ------------------------- |
| Operating System | Kali Linux 2025.x         |
| RAM              | 2.6 GB                    |
| CPU              | 2 Cores                   |
| Storage          | 80 GB                     |
| Vai trò        | Máy tấn công |

### Security Tools

* Hydra
* Nmap
* OpenSSH Client
* Linux Networking Utilities

# Vai trò của Virtual Machine

| Machine    | Primary Role       |
| ---------- | ------------------ |
| Ubuntu     | SIEM Server        |
| Windows 10 | Máy được giám sát |
| Linux      | Máy được giám sát |  
| Kali Linux | Máy tấn công  |

---
