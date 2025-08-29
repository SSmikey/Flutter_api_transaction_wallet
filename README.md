<div align="center">

# 💸 **Tangja Wallet**

<img src="https://img.shields.io/badge/Flutter-3.8.1-02569B?style=for-the-badge&logo=flutter" alt="Flutter" />
<img src="https://img.shields.io/badge/Dart-3.8.1-0175C2?style=for-the-badge&logo=dart" alt="Dart" />
<img src="https://img.shields.io/badge/GetX-4.7.2-9C27B0?style=for-the-badge" alt="GetX" />
<img src="https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge" alt="Status" />

<h3>📱 แอปพลิเคชันจัดการธุรกรรมทางการเงินส่วนบุคคล <br> <span style="color:#1976d2">พัฒนาโดย Flutter//</span></h3>

[🚀 การติดตั้ง](#-การติดตั้งและรัน) • [📱 ฟีเจอร์](#-ฟีเจอร์หลัก) • [🏗️ โครงสร้าง](#️-โครงสร้างโปรเจ็กต์) • [📋 API](#-api-documentation)

</div>

---

## 👨‍💻 ผู้พัฒนา

<div align="center">

👨‍💻 นายสิทธิชัย แสงนนท์ 6612732134  
👨‍💻 นายพีรพัฒน์ สุทธปัญญา 6612732121  
👨‍💻 นางสาววาสน มาฤทธ 6712732126  
👨‍💻 นางสาววรัญญา ฉิมงาม 6712732125

🏛️ สาขาวิทยาการคอมพิวเตอร์  
🎓 มหาวิทยาลัยราชภัฏศรีสะเกษ

</div>

---

## 📖 เกี่ยวกับโปรเจ็กต์

แอปพลิเคชันนี้ถูกออกแบบมาเพื่อจัดการบันทึกรายรับ-รายจ่ายส่วนบุคคลอย่างมีประสิทธิภาพ ด้วยเทคโนโลยี Flutter และแนวคิดการออกแบบที่ทันสมัย รองรับการเชื่อมต่อ RESTful API และจัดเก็บข้อมูลในเครื่องด้วย Hive Database พร้อมระบบยืนยันตัวตนที่ปลอดภัย

### 🌟 จุดเด่นสำคัญ

- ⚡ **Real-time Updates** — อัปเดตข้อมูลทันทีด้วย GetX
- 📶 **Offline Support** — ใช้งานได้แม้ไม่มีอินเทอร์เน็ต
- 🎨 **UI/UX ทันสมัย** — Material Design 3 & Custom Theme
- 🔒 **Authentication ปลอดภัย** — JWT Token
- 📝 **ฟังก์ชัน CRUD ครบถ้วน**

## 🎯 API ที่ใช้งาน

**Backend API:** [`https://transactions-cs.vercel.app`](https://transactions-cs.vercel.app)  
**GitHub Repository:** [Apisit250aps/transactions](https://github.com/Apisit250aps/transactions)

## 📱 ฟีเจอร์หลัก

### 🔐 **ระบบยืนยันตัวตน (Authentication)**

- 🚪 เข้าสู่ระบบด้วยอีเมลและรหัสผ่าน
- 📝 สมัครสมาชิกใหม่
- 🔑 รีเซ็ตรหัสผ่าน
- 🚪 ออกจากระบบ
- 🔒 ตรวจจับสถานะล็อกอินอัตโนมัติ

### 💸 **จัดการธุรกรรม (Transaction Management)**

- ➕ เพิ่มรายการรายรับ/รายจ่าย
- 📊 แสดงรายการธุรกรรมทั้งหมด
- ✏️ แก้ไขรายการ
- 🗑️ ลบรายการ
- 📅 เลือกวันที่ธุรกรรม
- 💰 แยกกระเป๋าตามประเภท

### 🎨 **UI/UX ทันสมัย**

- 🌈 Material Design 3
- 🎨 Custom Theme สีสันสวยงาม
- 📱 Responsive Design รองรับทุกอุปกรณ์
- ✅ Form Validation ตรวจสอบข้อมูล
- ⏳ Loading State
- ⚠️ Error Handling

### 🛠️ **เทคนิคเด่น**

- 🔄 State Management (GetX)
- 🗄️ Local Storage (Hive)
- 🌐 API Integration (HTTP)
- 🧭 Navigation (GetX Routing)
- 🔔 Real-time Updates

## 🏗️ โครงสร้างโปรเจ็กต์

```yaml
lib/
├── components/            # 🧩 คอมโพเนนต์ UI
│   ├── drawer.dart        # 📱 เมนูนำทาง
│   ├── transaction_card.dart # 💳 การ์ดแสดงธุรกรรม
│   └── user_profile_card.dart # 👤 โปรไฟล์ผู้ใช้
├── controllers/           # 🎮 ตัวควบคุม State
│   ├── auth_controller.dart    # 🔐 จัดการล็อกอิน
│   └── transac_controller.dart # 💸 จัดการธุรกรรม
├── model/                # 📊 โมเดลข้อมูล
│   └── transaction.dart      # 💰 โมเดลธุรกรรม
├── routes/               # 🧭 เส้นทางนำทาง
│   ├── app_pages.dart        # 📄 กำหนดเพจ
│   └── app_routes.dart       # 🛣️ ค่าคงที่เส้นทาง
├── screens/              # 📱 หน้าจอแอป
│   ├── splash_screen.dart    # 🌅 โหลดแอป
│   ├── login.dart            # 🔑 ล็อกอิน
│   ├── regis.dart            # 📝 สมัครสมาชิก
│   ├── forget_pass.dart      # 🔑 รีเซ็ตรหัสผ่าน
│   ├── home.dart             # 🏠 หน้าหลัก
│   └── transaction_form.dart # 📝 ฟอร์มธุรกรรม
├── services/             # ⚙️ เซอร์วิส
│   └── storage_service.dart  # 🗄️ จัดการ Local Storage
├── utils/                # 🛠️ ยูทิลิตี้
│   ├── api.dart              # 🌐 ตั้งค่า API
│   └── navigation_helper.dart # 🧭 ตัวช่วยนำทาง
└── main.dart              # 🚀 จุดเริ่มต้นแอป
```

## 🛠️ เทคโนโลยีที่ใช้

<div align="center">

| หมวดหมู่                | เทคโนโลยี     | เวอร์ชัน | วัตถุประสงค์          |
| ----------------------- | ------------- | -------- | --------------------- |
| 🎯 **Core**             | Flutter SDK   | `^3.8.1` | Framework หลัก        |
| 🎯 **Core**             | Dart          | `^3.8.1` | Programming Language  |
| 🎮 **State Management** | GetX          | `^4.7.2` | State, Routing & DI   |
| 🗄️ **Database**         | Hive          | `^2.2.3` | Local NoSQL Database  |
| 🌐 **HTTP Client**      | HTTP          | `^1.5.0` | API Communication     |
| 📁 **File System**      | Path Provider | `^2.1.4` | File Path Management  |
| 🧪 **Testing**          | Flutter Test  | Built-in | Unit & Widget Testing |
| 📋 **Code Quality**     | Flutter Lints | `^5.0.0` | Static Code Analysis  |

</div>

### 🏗️ รูปแบบสถาปัตยกรรม

- **📐 MVC** — Model-View-Controller
- **🎮 GetX** — State Management แบบ Reactive
- **📦 Repository** — แยกชั้นข้อมูล
- **🧩 Component-Based UI** — UI แบบนำกลับมาใช้ซ้ำ
- **🔄 Reactive Programming** — UI อัปเดตทันที

## 🚀 การติดตั้งและเริ่มต้นใช้งาน

### 📋 ความต้องการของระบบ

<div align="center">

| ⚙️ ระบบ            | 🔢 เวอร์ชันขั้นต่ำ     | 📝 หมายเหตุ                    |
| ------------------ | ---------------------- | ------------------------------ |
| 📱 **Flutter SDK** | `^3.8.1`               | Required                       |
| 🎯 **Dart SDK**    | `^3.8.1`               | มาพร้อม Flutter                |
| 💻 **IDE**         | Any                    | Android Studio / VS Code แนะนำ |
| 📱 **Platform**    | Android 6.0+ / iOS 12+ | สำหรับการทดสอบ                 |
| 🌐 **Internet**    | Required               | สำหรับ API Calls               |

</div>

### 📦 ขั้นตอนการติดตั้ง

```bash
# 1️⃣ โคลนโปรเจ็กต์
git clone https://github.com/your-username/api_consume.git
cd api_consume

# 2️⃣ ติดตั้ง Dependencies
flutter pub get

# 3️⃣ ตรวจสอบการติดตั้ง
flutter doctor

# 4️⃣ เริ่มต้นแอปพลิเคชัน
flutter run
```

### 🔧 การตั้งค่า

#### 🌐 API Configuration

ไฟล์ `lib/utils/api.dart` มีการตั้งค่า API Endpoint ดังนี้:

```dart
final BASE_URL = 'https://transactions-cs.vercel.app';

// Authentication Endpoints
final LOGIN_ENDPOINT = '/api/auth/login';
final REGISTER_ENDPOINT = '/api/auth/register';

// Transaction Endpoints
final TRANSACTION_ENDPOINT = '/api/transaction';
final CREATE_TRANSACTION_ENDPOINT = '/api/transaction';
```

#### 📁 การตั้งค่า Assets

กำหนด Assets ใน `pubspec.yaml`:

```yaml
flutter:
  uses-material-design: true
  assets:
    - assets/images/
```

**Assets ที่ใช้:**

- 🏛️ `comsci_logo.png` — โลโก้สาขาวิทยาการคอมพิวเตอร์
- 🎯 `logo.png` — โลโก้หลักของแอป
- 🔄 `reset.png` — ไอคอนรีเซ็ตรหัสผ่าน

## 📋 เอกสาร API

### 🔐 Authentication Endpoints

| Method | Endpoint             | Description | Body                      |
| ------ | -------------------- | ----------- | ------------------------- |
| `POST` | `/api/auth/login`    | เข้าสู่ระบบ | `{email, password}`       |
| `POST` | `/api/auth/register` | สมัครสมาชิก | `{name, email, password}` |

### 💰 Transaction Endpoints

| Method   | Endpoint                  | Description     | Headers                         |
| -------- | ------------------------- | --------------- | ------------------------------- |
| `GET`    | `/api/transaction`        | ดูรายการทั้งหมด | `Authorization: Bearer {token}` |
| `POST`   | `/api/transaction`        | เพิ่มรายการใหม่ | `Authorization: Bearer {token}` |
| `PUT`    | `/api/transaction/{uuid}` | แก้ไขรายการ     | `Authorization: Bearer {token}` |
| `DELETE` | `/api/transaction/{uuid}` | ลบรายการ        | `Authorization: Bearer {token}` |
## 🏗️ ฟีเจอร์โดยละเอียด

### 🎮 **Controllers**

#### 🔐 `AuthController` (`lib/controllers/auth_controller.dart`)

```dart
class AuthController extends GetxController {
  // 🚪 จัดการสถานะการเข้าสู่ระบบ
  // 🔑 เชื่อมต่อ API Login/Register/Reset Password
  // 💾 จัดเก็บ Token ใน Hive Local Storage
  // 🔄 Auto-login Detection เมื่อเปิดแอป
}
```

#### 💸 `TransactionController` (`lib/controllers/transac_controller.dart`)

```dart
class TransactionController extends GetxController {
  // 📊 จัดการ State ของรายการธุรกรรม
  // ➕ เพิ่มรายการใหม่ (addTransaction)
  // ✏️ แก้ไขรายการ (updateTransaction)
  // 🗑️ ลบรายการ (removeTransaction)
  // 🔄 Real-time Updates ด้วย RxList
}
```

