# 🌐 Enterprise Multi-Branch Network Design
> **Cisco Packet Tracer Simulation** | A comprehensive 3-branch enterprise infrastructure (Bangkok HQ, Phuket, and Chiang Mai).

---

## 📌 Project Overview
โปรเจกต์จำลองเครือข่ายระดับองค์กรที่เน้นความ **Scalable**  โดยเชื่อมต่อสำนักงานใหญ่และสาขาเข้าด้วยกันผ่านเทคโนโลยี Routing และ Switching 

## 🚀 Key Technical Features

### 🛣️ Routing & Connectivity
* **OSPF (Area 0):** โปรโตคอลการหาเส้นทางแบบ Dynamic เพื่อให้ทุกสาขาสื่อสารกันได้โดยอัตโนมัติและรวดเร็ว
* **Static Default Routing:** กำหนดทางออกอินเทอร์เน็ตที่ HQ เพื่อเป็น Gateway หลักขององค์กร
* **NAT Overload (PAT):** แปลง Private IP ภายในองค์กรให้เป็น Public IP เพื่อให้ทุกเครื่องเข้าถึง Web Server ภายนอกได้

### 🏢 Switching & Segmentations
* **VLAN Segmentation:** แบ่งแยกแผนกภายในเพื่อความปลอดภัยและลด Broadcast Traffic
    * `VLAN 10`: **Admin**
    * `VLAN 20`: **Sale**
* **Inter-VLAN Routing:** ใช้เทคนิค **802.1Q Router-on-a-Stick** เพื่อให้แต่ละแผนกสื่อสารกันได้ภายใต้การควบคุมของ Router

### 🛠️ Network Services
* **DHCP Server:** ตั้งค่า Localized Pools ในทุก Router เพื่อแจก IP Address ให้กับอุปกรณ์ปลายทางแยกตาม VLAN โดยอัตโนมัติ
* **DNS & Web Server:** จำลองระบบ Domain Name สำหรับการเข้าใช้งานเว็บไซต์ภายในและภายนอก

### 🔒 Security & Device Hardening
* **Access Security:** * ตั้งค่า `Enable Secret` สำหรับสิทธิ์การเข้าถึงระดับสูงสุด
    * ตั้งรหัสผ่านสำหรับ `Line Console` และ `VTY` (Remote Access)
* **Data Protection:** เปิดใช้งาน `Service Password-Encryption` เพื่อเข้ารหัสทุก Password ในไฟล์ Config
* **Access Warnings:** ตั้งค่า `Custom Banner MOTD` เพื่อแจ้งเตือนการเข้าถึงโดยไม่ได้รับอนุญาต

---

## 📊 Network Topology
![Network Topology](https://github.com/user-attachments/assets/73fedb45-df0a-4ccf-a31f-4836dc005ddf)



---
**Developed by:** Supakit Chusing (CE MFU)
