# MACOC
### Official Package Manager for Dolet

`macoc` هو مدير الحزم الرسمي لمشاريع **Dolet**.
مصمم ليكون خفيفًا، سريعًا، ومكتوب بالكامل بلغة **Pure Dolet** بدون أي اعتماد خارجي.

> ⚡ Native. Fast. Minimal.
> Built for the Dolet ecosystem.

---

## ✨ Features

- 🚀 سرعة تنفيذ عالية
- 📦 تثبيت وإزالة الحزم بسهولة
- 🧩 إدارة الاعتماديات الخارجية
- 🛠️ مكتوب بالكامل بـ Pure Dolet
- 🔒 تصميم بسيط ومستقر
- 🌍 يعمل على Linux و Windows

---

## 📦 Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/macoc.git
cd macoc
```

---

### 2️⃣ Build

#### باستخدام مترجم Dolet مباشرة

```bash
dolet main.dlt -o macoc
```

#### أو باستخدام سكربتات البناء

**Linux**
```bash
./linux_build.sh
```

**Windows**
```bash
.\windows_build.bat
```

---

## ➕ Add macoc to PATH

### 🐧 Linux / macOS

أفضل طريقة:

```bash
sudo mv macoc /usr/local/bin/
```

أو أضف مساره يدويًا:

```bash
export PATH="$PATH:/path/to/macoc"
```

---

### 🪟 Windows

1. افتح *Edit the system environment variables*
2. اضغط **Environment Variables**
3. عدّل متغير **Path**
4. أضف مسار المجلد الذي يحتوي على `macoc.exe`
5. اضغط OK

---

## ⚡ Quick Start

بعد الإعداد يمكنك استخدامه من أي مجلد:

```bash
macoc
```

تثبيت حزمة:

```bash
macoc install <package_name>
```

إزالة حزمة:

```bash
macoc remove <package_name>
```

---

## 📁 Project Structure

```
macoc/
 ├── main.dlt
 ├── linux_build.sh
 ├── windows_build.bat
 └── README.md
```

---

## 🧠 Design Philosophy

`macoc` يتبع مبادئ Dolet:

- أداء عالٍ بدون تعقيد
- لا اعتماديات خارجية
- وضوح في التنفيذ
- تحكم كامل على مستوى النظام

الهدف هو إبقاء مدير الحزم بسيطًا وسريعًا بدل تحويله إلى نظام ضخم ومعقد.

---

## 🔮 Roadmap

- [ ] دعم versioning متقدم
- [ ] دعم dependency resolution
- [ ] registry مركزي للحزم
- [ ] lock file للنُسخ الثابتة
- [ ] دعم مشاريع متعددة داخل workspace

---

## 🤝 Contributing

المساهمات مرحب بها.

1. Fork المشروع
2. أنشئ branch جديد
3. أضف تعديلاتك
4. افتح Pull Request

---

## 📜 License

MIT License
Free to use, modify, and distribute.

---

## 💬 About Dolet

Dolet هي لغة برمجة عالية الأداء تركز على:

- توليد Machine Code مباشر
- أداء يشبه Rust
- نظام أنواع صارم
- تصميم minimal بدون overhead

`macoc` هو جزء من منظومة أدوات Dolet الرسمية.

---

# 🚀 Why macoc?

لأن لغة قوية تحتاج مدير حزم بنفس القوة.


# NOTE RN THE PROJECT IS WORKS WITH WINDOWS COS THE SOURCE CODE USING THE DIRECTLY WIN API, LATER WE WILL MAKE ANOTHER FFI FILE AND DEFINE FUNCTIONS TO MAKE THEM USE THE WIN API (KERNEL32 FOR WINDOWS) OR THE SYSCALL FOR LINUX AND SAME THING WITH OTHERS TO MAKE IT CROSSPLATFORM.