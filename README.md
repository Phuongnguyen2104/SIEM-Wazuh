<h1 align="center">
SIEM-Based Cybersecurity Monitoring Using Wazuh
</h1>

<p align="center">
Triển khai hệ thống SIEM doanh nghiệp sử dụng Wazuh để thu thập nhật ký (log) tập trung, giám sát tính toàn vẹn của tệp (File Integrity Monitoring - FIM), giám sát bảo mật điểm cuối (Endpoint Security Monitoring), mô phỏng các cuộc tấn công, xây dựng các quy tắc phát hiện tùy chỉnh (Custom Detection Rules) và phân tích các sự kiện bảo mật (Security Event Analysis).
</p>

<p align="center">
  
![Wazuh](https://img.shields.io/badge/Wazuh-SIEM-0052CC?style=for-the-badge&logo=wazuh&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu-22.04-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![Windows](https://img.shields.io/badge/Windows-10-0078D4?style=for-the-badge&logo=windows&logoColor=white)
![Kali Linux](https://img.shields.io/badge/Kali-Linux-268BEE?style=for-the-badge&logo=kalilinux&logoColor=white)
![VMware](https://img.shields.io/badge/VMware-Workstation-607078?style=for-the-badge&logo=vmware&logoColor=white)
![Nmap](https://img.shields.io/badge/Nmap-Network%20Scanner-00457C?style=for-the-badge)
![Hydra](https://img.shields.io/badge/Hydra-Brute%20Force-8A2BE2?style=for-the-badge)
![XML](https://img.shields.io/badge/XML-Custom%20Rules-FF6600?style=for-the-badge)
![MIT License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

</p>

---

## 📌 Project Overview

Dự án này trình bày việc triển khai một giải pháp Quản lý Thông tin và Sự kiện Bảo mật (Security Information and Event Management - SIEM) cấp doanh nghiệp sử dụng Wazuh trong một phòng thí nghiệm an ninh mạng được ảo hóa. Môi trường triển khai bao gồm một máy chủ Wazuh chạy Ubuntu, một máy agent Windows 10, một máy agent linux và một máy Kali Linux đóng vai trò máy tấn công, được kết nối thông qua một mạng ảo cách ly.

Dự án tập trung vào việc giám sát hoạt động của các endpoint, thu thập nhật ký bảo mật (security logs), phát hiện các cuộc tấn công mạng, xây dựng các quy tắc phát hiện tùy chỉnh (custom detection rules) và phân tích các sự kiện bảo mật thông qua Wazuh Dashboard.

---

## 🏗️ Solution Architecture
Sơ đồ kiến ​​trúc sau đây minh họa việc triển khai môi trường giám sát an ninh mạng dựa trên SIEM được thực hiện trong dự án này.


### Architecture Overview
- Máy chủ Ubuntu Wazuh Server là nơi lưu trữ Wazuh Manager, Indexer và Dashboard.
- Windows 10 đóng vai trò là thiết bị đầu cuối được giám sát với phần mềm Wazuh Agent đã được cài đặt.
- Kali Linux được sử dụng để mô phỏng các cuộc tấn công mạng, bao gồm cả hoạt động trinh sát Nmap và các cuộc tấn công vét cạn mật khẩu SSH bằng Hydra.
- Máy chủ Wazuh thu thập, phân tích và hiển thị trực quan các sự kiện bảo mật trong thời gian thực.
- Các quy tắc tùy chỉnh của Wazuh phát hiện các lỗi đăng nhập SSH và các nỗ lực tấn công vét cạn, tạo ra các cảnh báo ưu tiên cao.

## 🎯 Objectives
- Triển khai nền tảng SIEM tập trung bằng Wazuh
- Cấu hình thu thập nhật ký tập trung
- Triển khai tính toàn vẹn của tập tin (FIM)
- Giám sát các thiết bị đầu cuối Windows và Linux
- Mô phỏng các cuộc tấn công mạng trong thế giới thực.
- Tạo các quy tắc phát hiện Wazuh tùy chỉnh
- Phân tích các sự kiện bảo mật bằng cách sử dụng Bảng điều khiển Wazuh.

## 🛠 Technologies Used
- Wazuh SIEM
- Ubuntu Linux
- Windows 10
- Kali Linux
- VMware Workstation
- XML
- SSH
- Nmap
- Hydra
- Linux Administration

## 📂 Project Structure


## 🔐 Implemented Modules

