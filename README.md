# 🍜 FoodDelivery - เวอร์ชันพร้อมใช้งาน (Path แก้แล้ว)

## ✅ ไฟล์นี้พร้อมอัปโหลดไปยัง GitHub Pages แล้ว!

ผมได้แก้ไข path ของ CSS และ JavaScript ให้ถูกต้องแล้ว

---

## 📁 โครงสร้างไฟล์

```
food-delivery-simple/
├── index.html          ← หน้าแรก
├── login.html          ← เข้าสู่ระบบ
├── register.html       ← สมัครสมาชิก
├── menu.html           ← เมนูอาหาร
├── cart.html           ← ตะกร้าสินค้า
├── checkout.html       ← ชำระเงิน
├── orders.html         ← รายการสั่งซื้อ
├── tracking.html       ← ติดตามออเดอร์
├── profile.html        ← โปรไฟล์
├── main.css            ← ไฟล์ CSS (แก้ path แล้ว)
├── main.js             ← ไฟล์ JavaScript (แก้ path แล้ว)
└── images/             ← โฟลเดอร์รูปภาพ (ว่างเปล่า - ต้องเพิ่มเอง)
```

---

## 🚀 วิธีอัปโหลดไปยัง GitHub

### วิธีที่ 1: ผ่าน GitHub Web (ง่ายที่สุด)

1. **ไปที่ repository ของคุณบน GitHub**
   ```
   https://github.com/username/repository-name
   ```

2. **อัปโหลดไฟล์ทั้งหมด:**
   - คลิก **"Add file"** → **"Upload files"**
   - ลากไฟล์ทั้งหมดในโฟลเดอร์นี้มาวาง (รวมโฟลเดอร์ images/)
   - เขียน commit message: "Upload FoodDelivery website"
   - คลิก **"Commit changes"**

3. **ตั้งค่า GitHub Pages:**
   - ไปที่ **Settings** → **Pages**
   - Source: **Deploy from a branch**
   - Branch: **main** → **/root**
   - คลิก **Save**

4. **รอ 1-2 นาที** แล้วเปิดที่:
   ```
   https://username.github.io/repository-name/
   ```

### วิธีที่ 2: ผ่าน Git Command Line

```bash
# 1. Clone repository
git clone https://github.com/username/repository-name.git
cd repository-name

# 2. คัดลอกไฟล์ทั้งหมดมาวาง

# 3. Add และ commit
git add .
git commit -m "Upload FoodDelivery website with fixed paths"
git push origin main
```

---

## 🖼️ เพิ่มรูปภาพอาหาร

คุณต้องเพิ่มรูปภาพเหล่านี้ในโฟลเดอร์ `images/`:

### รายการรูปที่ต้องการ:
1. **padthai.jpg** - ผัดไทยกุ้งสด
2. **tomyum.jpg** - ต้มยำกุ้ง
3. **fried-rice.jpg** - ข้าวผัดกุ้ง
4. **burger.jpg** - เบอร์เกอร์ชีส
5. **pizza.jpg** - พิซซ่า
6. **fried-chicken.jpg** - ไก่ทอด
7. **sushi.jpg** - ซูชิ
8. **ramen.jpg** - ราเมง
9. **chocolate-cake.jpg** - เค้กช็อกโกแลต
10. **icecream.jpg** - ไอศกรีม
11. **green-tea.jpg** - ชาเขียว
12. **iced-coffee.jpg** - กาแฟเย็น
13. **Noodle.jpg** - รูป fallback

### หาไฟล์รูปได้จาก:
- 🔍 Google Images (ค้นหา "food photography")
- 🌅 [Unsplash](https://unsplash.com/s/photos/food) - รูปฟรีคุณภาพสูง
- 🍔 [Pexels](https://www.pexels.com/search/food/) - รูปฟรี
- 🎨 [Pixabay](https://pixabay.com/images/search/food/) - รูปฟรี

### หรือใช้รูป Placeholder ชั่วคราว:
ถ้ายังไม่มีรูป เว็บจะแสดงอีโมจิอาหารแทน (มีในโค้ดอยู่แล้ว) 🍴

---

## ✅ ตรวจสอบว่าใช้งานได้

### 1. เปิด Browser Console (กด F12)
- ไปที่แท็บ **Network**
- Reload หน้าเว็บ (กด F5)
- ดูว่า `main.css` และ `main.js` โหลดสำเร็จ
- ถ้าเห็น **200** (สีเขียว) = สำเร็จ ✅
- ถ้าเห็น **404** (สีแดง) = มีปัญหา ❌

### 2. ตรวจสอบหน้าเว็บ
- ✅ หน้าเว็บมีสีสัน มีการจัดรูปแบบสวยงาม
- ✅ ปุ่มต่างๆ ทำงานได้ (เพิ่มตะกร้า, ล็อกอิน)
- ✅ เมนูด้านบนแสดงผล
- ✅ Footer แสดงผล

---

## 🔧 แก้ไขที่ทำไปแล้ว

ผมได้แก้ไขสิ่งเหล่านี้แล้ว:

### ✅ Path ของ CSS:
```html
<!-- เดิม -->
<link rel="stylesheet" href="../css/main.css">

<!-- แก้เป็น -->
<link rel="stylesheet" href="main.css">
```

### ✅ Path ของ JavaScript:
```html
<!-- เดิม -->
<script src="../js/main.js"></script>

<!-- แก้เป็น -->
<script src="main.js"></script>
```

### ✅ Path ของรูปภาพ:
```html
<!-- เดิม -->
<img src="../images/burger.jpg">

<!-- แก้เป็น -->
<img src="images/burger.jpg">
```

---

## 🐛 แก้ปัญหา

### ปัญหา: CSS ยังไม่โหลด
**แก้:**
- ตรวจสอบว่าไฟล์ `main.css` อยู่ที่ root ของ repository
- ลอง hard reload: **Ctrl + Shift + R** (Windows) หรือ **Cmd + Shift + R** (Mac)
- รอ 1-2 นาที (GitHub Pages ต้อง build)

### ปัญหา: JavaScript ไม่ทำงาน
**แก้:**
- ตรวจสอบว่าไฟล์ `main.js` อยู่ที่ root
- เปิด Console (F12) ดู error
- ตรวจสอบ Browser รองรับ JavaScript

### ปัญหา: รูปภาพไม่แสดง
**แก้:**
- เพิ่มรูปภาพลงในโฟลเดอร์ `images/`
- ตรวจสอบชื่อไฟล์ให้ตรง (case-sensitive)
- หรือเว็บจะแสดงอีโมจิแทน (ซึ่งก็ดูได้)

---

## 💡 Tips

1. **ทดสอบ Local ก่อน:** เปิดไฟล์ `index.html` ในเครื่องดูก่อนว่าทำงานหรือไม่
2. **ใช้ Live Server:** ถ้าใช้ VS Code ติดตั้ง Live Server extension
3. **ตั้งชื่อให้ถูก:** GitHub Pages case-sensitive (Burger.jpg ≠ burger.jpg)
4. **Clear Cache:** ถ้าแก้แล้วไม่เห็นผล ลอง Incognito mode

---

## 📞 ติดต่อ

- 📧 Email: eprrequiem@gmail.com
- 📱 Tel: 065-921-9022

---

## 📝 สิ่งที่เปลี่ยนแปลง

### Version 2.1 (2026-01-31)
- ✅ แก้ไข path ของ CSS จาก `../css/main.css` → `main.css`
- ✅ แก้ไข path ของ JS จาก `../js/main.js` → `main.js`
- ✅ แก้ไข path ของรูปภาพ จาก `../images/` → `images/`
- ✅ พร้อมอัปโหลดไปยัง GitHub Pages ได้ทันที

---

**🎉 พร้อมใช้งานแล้ว! ขอให้สนุกกับการสั่งอาหารออนไลน์!**
