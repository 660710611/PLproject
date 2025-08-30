# Changing a Section of a String 
    เป็นการใช้เมธอดต่างๆกับสตริง ซึ่งทำให้สตริงเกิดการเปลี่ยนแปลงโดยที่ไม่ได้เกิดจาการสร้างสตริงใหม่
  ##### โดยมีวิธีการพื้นฐาน ดังนี้ 
   
## สารบัญ Table of Contents

 - String Slices
  - Substitution Methods
    - sub && sub!
    - gsub && gsub!

## วิธีการ Changing a Section of a String 
### String Slice 
    เป็นเมธอดที่ใช้ในการเปลี่ยนแปลงคำในสตริง โดยใช้สัญลักษณ์[]
#### ตัวอย่าง
    
   ```
myString = "Silpakorn University"
puts 'mySring'[0] 

```
คอมเม้นว่า เริ่มนับยังไง 
 ####  ทำ dropdown output 
  #####  อธิบาย  แต่ถ้าไม่มีเท่ากับจะไม่แปลงค่า
   ```
myString = "Silpakorn University"
myString["University"] = "Educator"
puts myString

```
  
    แบบแปลงแทนที่คำในสตริงโดยตรง
    แปลงโดยอิงจากอินเด็ก
   ```
myString = "Silpakorn University"
myString[9] = " is "
puts myString

```
    แปลงโดยอิงจากช่วงค่าอินเดก
    ใส่ตัวอย่าง 
    ละก้ใส่ตัวอย่างจาก c python java
### Substitution Methods
    นิยามรวม
    แบ่งออกเป็น 2 วิธี ได้แก่
    1.sub && sub!
      นิยาม
      ตัวอย่าง
      เทียบกับ c python java
    2.gsub && gsub!
      นิยาม
      ตัวอย่าง
      เทียบกับ c python java
  
## เครดิต

```
myString = "Silpakorn University"
puts 'mySring'[0]

```