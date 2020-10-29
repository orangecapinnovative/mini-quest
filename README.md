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

โดยที่เว็บไซต์ไม่จำเป็นต้องมี Link / Interaction ขอแค่ให้หน้าตาตรงกันหรือใกล้เคียง และ Responsive ทั้ง Mobile และ Desktop และรูปภาพสามารถโหลดได้จากเว็บไซต์ของ GitHub ได้เลย

## 2. JavaScript / TypeScript + Algorithm

ส่วนนี้จะมีโจทย์ย่อย 3 ข้อ โดยจะเป็นการทดสอบพื้นฐานการใช้งานภาษา JavaScript (หรือ TypeScript ก็ได้) ผนวกกับทดสอบความรู้ Algorithm โค้ดทั้งหมดจะถูกรันโดย Node.js ดังนั้นควรเช็คให้ดีก่อนจะส่งมานะค้าบ

1. **Second Max** ให้เขียนฟังก์ชัน `secondMax(arr: number[]) => number` ที่รับ Array มา แล้วคืนค่าสูงสุดอันดับสองมาให้ ในกรณีที่ไม่มีค่าสูงสุดอันดับสอง ให้คืนค่าสูงสุดมาแทน และในกรณีที่ส่ง Array เปล่ามา ให้แสดงผล Error แทน

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

2. **Fibonacci**: เขียนฟังก์ชัน `fib(n: number) => number` ที่รับ integer ที่มีค่ามากกว่า 1 ขึ้นมา ฟังก์ชันจะต้องคืนค่าลำดับ Fibonacci ลำดับที่ n

ลำดับ Fibonacci เกิดจากการนำลำดับสองตัวก่อนหน้าบวกค่ากัน โดยลำดับนี้จะเริ่มที่ 1, 1 ทำให้ลำดับ Fibonacci จะมีเลขตามด้านล่างนี้

```
1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, ...
```

```js
> fib(1)
1

> fib(3)
2

> fib(12)
144
```

3. **Common Character Count**: เขียนฟังก์ชัน `commonCharacterCount(s1: string, s2: string) => number` ที่รับ string 2 ชุดมา ฟังก์ชันจะคืนค่าว่ามีจำนวนตัวอักษรที่พบได้ใน string ทั้งสองรวมกันกี่ตัว โดยตัวอักษรที่ตรงกันไม่จำเป็นต้องสนใจลำดับ

เช่น

- `aabcd` กับ `abaef` จะได้ผลลัพธ์เป็น 3 เพราะ a 2 ตัวอักษร และ b 1 ตัวอักษร ที่ปรากฎขึ้นทั้งสอง string รวมกันทั่้งหมดเป็น 3
- `aaa` กับ `bbb` ได้ผลลัพธ์เป็น 0 เพราะไม่มีตัวอักษรปรากฎร่วมกัน
- `aab` กับ `ae` ได้ผลลัพธ์เป็น 1 เพราะมี a ปรากฎตัวเหมือนกัน 1 ตัวอักษรเท่านั้น

4. **Almost Increasing Sequence**: เขียนฟังก์ชัน `almostIncreasingSequence(arr: number[]) => boolean` ที่รับ array ของ integer มา 1 ชุด โดยจะคืนค่า boolean ว่า ลำดับที่ได้มา เป็นลำดับที่สามารถเพิ่มขึ้นอย่างเดียวได้ไหม โดยที่สามารถดึงสมาชิกใน array ออกได้อย่างมาก 1 ตัว

เช่น

- `[1, 2, 3]` ได้ผลลัพธ์เป็น true เนื่องจากลำดับนี้มีค่าเพิ่มขึ้นเรื่อยๆ
- `[1, 3, 2]` ได้ผลลัพธ์เป็น true แม้ว่าลำดับดั้งเดิมจะไมได้มีค่าเพิ่มขึ้นเรื่อยๆ แต่ถ้าหากเราลบเลข 3 ออกจาก array จะได้ `[1, 2]` ซึ่งเป็นลำดับที่มีค่าเพิ่มขึ้นเรื่อยๆ หรือจะเลือกถอด 2 ก็จะได้ `[1, 3]` ซึ่งก็เป็นลำดับที่มีค่าเพิ่มขึ้นเรื่อยๆ เช่นกัน
- `[1, 3, 2, 1]` ได้ผลลัพธ์เป็น false เพราะลำดับดั้งเดิมจะไม่ได้มีค่าเพิ่มขึ้นเรื่อยๆ ถึงแม้เราจะลองลบเลขออกจาก array แบบไหนก็ตาม (`[3, 2 ,1]`, `[1, 2, 1]`, `[1, 3, 1]`, `[1, 3 ,2]`) ก็จะไม่ได้ลำดับที่มีค่าเพิ่มขึ้นเรื่อยๆ  จึงได้ผลลัพธ์เป็น false

```js
> almostIncreasingSequence([1, 2, 3])
true

> almostIncreasingSequence([1, 3, 2])
true

> almostIncreasingSequence([1, 3, 2, 1])
false
```

## 3. Front-end Development with React

ทำแอพ Todo List โดยใช้ React (https://reactjs.org/) โดยที่ Todo List นั้นมีฟีเจอร์ดังต่อไปนี้

- สามารถเพิ่ม Todo ได้
- สามารถลบ Todo ได้
- Todo สามารถ Mark as done / Unmark as done ได้
- สามารถ Filter ได้ว่าจะดูรายการ Todo ที่ Done แล้ว กับยังไม่ Done หรือดูทุกอัน
- Todo ทุกอันจะเรียงตามเวลาสร้าง โดยเอาอันที่สร้างใหม่สุดไว้ด้านบน
- Design สามารถเสกได้เต็มที่
- สามารถเลือกใช้ tools ไหนในการสร้างโปรเจคก็ได้ เช่น create-react-app / Next.js ตราบใดที่โค้ดยังเป็นโค้ด React อยู่

## 4. Back-end Development with Express / Mongoose

ทำ REST API สำหรับระบบ Todo List โดยใช้ Express (https://expressjs.com/) คู่กับ Mongoose (https://mongoosejs.com/) เป็นฐานข้อมูล

โดยที่ REST API Todo List จะต้องมีัฟีเจอร์ต่อไปนี้

- มีระบบ User ที่สามารถ Sign Up / Login ด้วย E-mail และ Password ได้
- กำหนดกฎของ Password ได้เองเลยตามความเหมาะสม
- สามารถดู Todo List ที่ตัวเองสร้างไว้ได้
- สามารถเพิ่ม Todo ได้
- สามารถลบ Todo ได้
- Todo สามารถ Mark as done ได้
- API สำหรับการเรียกดู Todo List ต้องรองรับการ filter ตาม status ว่าจะดูเฉพาะที่ Done แล้ว หรือยังไม่ Done หรือดูทุกอัน


## Bonus ทำเพิ่มก็ได้ ไม่ทำก็ได้

หากทำทั้งข้อ 3 และ 4 เสร็จ สามารถทำข้อนี้ได้ โดยนำโจทย์ข้อ 3 มาเชื่อมกับ API หลังบ้านข้อ 4 เพื่อสร้าง Todo List App ที่มีระบบ Login พร้อมกับบันทึกค่าต่างๆ ลงฐานข้อมูลได้เลย
