# TakeMeTour Mini Quest

## Tools ที่ควรติดตั้งเตรียมไว้

- Node.js https://nodejs.org/en/

## รายละเอียดโจทย์

โจทย์นี้จะมีทั้งหมด 4 ข้อ โดยไต่ระดับความยากและความซับซ้อน ให้ทำโจทย์ไล่ตามลำดับมา **อย่าทำข้ามข้อ** โจทย์ทั้ง 4 ข้อจะมีหัวข้อดังนี้

1. HTML + CSS
2. JavaScript / TypeScript + Algorithm
3. Front-end Development with React
4. Back-end Development with Express / Mongoose

โดยข้อ 3 และ 4 **สามารถเลือกทำได้ตามความสนใจ** หรือจะทำทั้งคู่ก็ย่อมได้

## 1. HTML + CSS

ให้ทำการเขียน HTML และ CSS ขึ้นมา 1 หน้า ที่มี Design ตามรูปด้านล่าง ซึ่งเป็นเว็บไซต์ GitHub (https://github.com/) หน้าแรกฉบับย่อที่ตัดบางส่วนออกไป

![./github.png](./github.png)
Desktop Size

![./github_ipad.png](./github_ipad.png)
iPad Size

![./github_mobile.png](./github_mobile.png)
Mobile Size

โดยที่เว็บไซต์ไม่จำเป็นต้องมี Link / Interaction ขอแค่ให้หน้าตาตรงกันหรือใกล้เคียง และ Responsive ทั้ง Mobile และ Desktop

## 2. JavaScript / TypeScript + Algorithm

ส่วนนี้จะมีโจทย์ย่อย 3 ข้อ โดยจะเป็นการทดสอบพื้นฐานการใช้งานภาษา JavaScript (หรือ TypeScript ก็ได้) ผนวกกับทดสอบความรู้ Algorithm โค้ดทั้งหมดจะถูกรันโดย Node.js ดังนั้นควรเช็คให้ดีก่อนจะส่งมานะค้าบ

1. **Second Max** ให้เขียนฟังก์ชัน `secondMax` ที่รับ Array มา แล้วคืนค่าสูงสุดอันดับสองมาให้ ในกรณีที่ไม่มีค่าสูงสุดอันดับสอง ให้คืนค่าสูงสุดมาแทน และในกรณีที่ส่ง Array เปล่ามา ให้แสดงผล Error แทน

```js
> secondMax([2, 3, 4, 5])
4

> secondMax([9, 2, 21, 21])
9

> secondMax([4, 4, 4, 4])
4

> secondMax([4123])
4123

> secondMax([])
Error!
```

2. **Character Checker** (โจทย์นี้ inspire จาก https://beta.programming.in.th/tasks/0004) ให้เขียนฟังก์ชัน `characterChecker` ที่รับ String มา โดย String ที่ส่งมานั้น จะประกอบไปด้วย `a-z` `A-Z` ฟังก์ชันจะคืนค่าได้ 3 กรณี

- ถ้า String ที่เข้ามามีแต่ตัวพิมพ์ใหญ่หมด เช่น ABCDOIAOSA ให้คืนคำว่า "All Capital Letter"
- ถ้า String ที่เข้ามามีแต่ตัวพิมพ์เล็กหมด เช่น aelkddnks ให้คืนคำว่า "All Small Letter"
- ถ้า String ที่เข้ามามีทั้งพิมพ์ใหญ่และเล็ก เช่น AKsdsEloa ให้คืนคำว่า "Mix"

```
> characterChecker('ABCDOIAOSA')
All Capital Letter

> characterChecker('aelkddnks')
All Small Letter

> characterChecker('AKsdsEloa')
Mix
```



## 3. Front-end Development with React

ทำแอพ Todo List โดยใช้ React (https://reactjs.org/) โดยที่ Todo List นั้นมีฟีเจอร์ดังต่อไปนี้

- สามารถเพิ่ม Todo ได้
- สามารถลบ Todo ได้
- Todo สามารถ Mark as done ได้
- สามารถ Filter ได้ว่าจะดูรายการ Todo ที่ Done แล้ว กับยังไม่ Done หรือดูทุกอัน
- Todo ทุกอันจะเรียงตามเวลาสร้าง โดยเอาอันที่สร้างใหม่สุดไว้ด้านบน
- Design สามารถเสกได้เต็มที่

## 4. Back-end Development with Express / Mongoose
