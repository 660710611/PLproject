###
# Changing a Section of a String 

 >  เป็นการใช้เมธอดต่างๆกับสตริง ซึ่งทำให้สตริงเกิดการเปลี่ยนแปลงโดยที่ไม่ได้เกิดจากการสร้างสตริงใหม่
  #### โดยมีวิธีการพื้นฐาน ดังนี้ 
   
## สารบัญ Table of Contents

 - String Slices
  - Substitution Methods
    - sub && sub!
    - gsub && gsub!
 - เปรียบเทียบกับภาษาอื่นๆ

## วิธีการ Changing a Section of a String 
### String Slice 
   >เป็นเมธอดที่ใช้ในการเปลี่ยนแปลงคำในสตริง โดยใช้สัญลักษณ์[]
#### ตัวอย่าง
   ```ruby
myString = "Silpakorn University"
puts 'mySring'[0] 

```
คอมเม้นว่า เริ่มนับยังไง 
<details>
   <summary>Output</summary>

    c value: 1  
    b value: 1  

</details>
  #####  อธิบาย  แต่ถ้าไม่มีเท่ากับจะไม่แปลงค่า

```ruby
myString = "Silpakorn University"
myString["University"] = "Educator"
puts myString

```
<details>
   <summary>Output</summary>

    c value: 1  
    b value: 1  

</details>
 
 > แบบแปลงแทนที่คำในสตริงโดยตรง
    
   ```ruby
myString = "Silpakorn University"
myString[9] = " is "
puts myString

```
<details>
   <summary>Output</summary>

    c value: 1  
    b value: 1  

</details>
   

 >แปลงโดยอิงจากอินเด็ก
```ruby
myString = "Silpakorn University"
myString[9...25] = "is The Best "
puts myString
```
<details>
   <summary>Output</summary>

    c value: 1  
    b value: 1  

</details>

> แปลงโดยอิงจากช่วงค่าอินเดก
> 
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

สรุปก่อนนะ: **Ruby สามารถแก้ไข string แบบ _mutable_ ได้ (string slice แล้วเปลี่ยนค่าได้เลย)**  
แต่ในหลายภาษา string เป็น **immutable (แก้ตรง ๆ ไม่ได้)** → ต้องใช้วิธีอื่นแทน
Ruby อนุญาตให้แก้ไขค่าใน string ได้โดยตรง