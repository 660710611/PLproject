###
# Changing a Section of a String 

 >  เป็นการใช้เมธอดต่างๆกับสตริง ซึ่งทำให้สตริงเกิดการเปลี่ยนแปลงโดยที่ไม่ได้เกิดจากการสร้างสตริงใหม่ #เพิ่มเติม
  #### โดยมีวิธีการพื้นฐาน ดังนี้ 
   
## สารบัญ Table of Contents

 - String Slices
  - Substitution Methods
    - String#sub &&  String#sub!
    - String#gsub &&  String#gsub!
 - เปรียบเทียบกับภาษาอื่นๆ

## วิธีการ Changing a Section of a String 
## String Slice 
   >เป็นเมธอดที่ใช้ในการเปลี่ยนแปลงคำในสตริง โดยใช้สัญลักษณ์[] #แก้
#### ตัวอย่าง
   ```ruby
myString = "Silpakorn University"
puts 'myString'[0] 
# เริ่มนับจากตัวอักษรแรก เป็นตำแหน่งที่ 0
```
<details>
   <summary>Output</summary>

    > S

</details>

>  อธิบาย  แต่ถ้าไม่มีเท่ากับจะไม่แปลงค่า #แก้

```ruby
myString = "Silpakorn University"
myString["University"] = "Educator"
puts myString

```
<details>
   <summary>Output</summary>

    > Silpakorn Educator

</details>
 
 > แบบแปลงแทนที่คำในสตริงโดยตรง
    
   ```ruby
myString = "Silpakorn University"
myString[9] = " is "
puts myString

```
<details>
   <summary>Output</summary>

    > Silpakorn is University

</details>
   

 >แปลงโดยอิงจากอินเด็ก
```ruby
myString = "Silpakorn University"
myString[9...20] = " is The Best "
puts myString
#นับตั้งแต่ตัวอักษรตัวที่ 9 ถึง ตัวที่ 25 
#แม้ช่องจะเกินก็ไม่เป็นอะไร ขอแค่เริ่มต้นที่
```
<details>
   <summary>Output</summary>
   
     > Silpakorn is The Best 

</details>

> แปลงโดยอิงจากช่วงค่าอินเดก

## Substitution Methods
   > นิยามรวม
   
   ### แบ่งออกเป็น 2 วิธี ได้แก่
   - String#sub &&  String#sub!
      นิยาม
      ตัวอย่าง
      เทียบกับ c python java
      
    - String#gsub &&  String#gsub!
      นิยาม
      ตัวอย่าง
      เทียบกับ c python java
  
  ใส่ตัวอย่าง 
    ละก้ใส่ตัวอย่างจาก c python java
## เครดิต

สรุปก่อนนะ: **Ruby สามารถแก้ไข string แบบ _mutable_ ได้ (string slice แล้วเปลี่ยนค่าได้เลย)**  
แต่ในหลายภาษา string เป็น **immutable (แก้ตรง ๆ ไม่ได้)** → ต้องใช้วิธีอื่นแทน
Ruby อนุญาตให้แก้ไขค่าใน string ได้โดยตรง