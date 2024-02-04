# Web Development Tools

เครื่องมือสำหรับการพัฒนาเว็บไซต์ (Web Development Tools) เป็นเครื่องมือที่ช่วยให้นักพัฒนาเว็บ สามารถที่จะทดสอบ หรือ Debug เว็บไซต์ที่พัฒนาขึ้นมาได้ โดยนักพัฒนาส่วนมากมักจะเลือกพัฒนาตัวเว็บโดยใช้ Website Builders หรือพัฒนาใน Integrated Development Environment (IDE) ซึ่งเป็นเครื่องมือที่ช่วยในการเขียนโค๊ด หรือทดสอบ Source Code เเต่ในการพัฒนาเว็บในบางครั้งนักพัฒนาก็จะต้องมีเครื่องมือเฉพาะสำหรับเว็บ ที่ใช้ในการทดสอบ หรือ Debug ในเเต่ละส่วน หรือเเต่ละ Element บนเว็บ โดยในการพัฒนาเว็บไซต์หลักๆ จะประกอบไปด้วยเครื่องมือดังนี้

1.  เว็บบราวเซอร์ (Web Browser)
2.  เว็บเซิฟเวอร์ (Web Server)
3.  ภาษาเขียนโปรเเกรม (Programming Language)
4.  โปรเเกรมสำหรับเขียนโค๊ด (Integrated Development Environment)

## 1. เว็บบราวเซอร์ (Web Browser)

โปรแกรมที่ใช้ในการเข้าถึงข้อมูลและติดต่อสื่อสารในรูปแบบเว็บเพจ (Web Page) โดยโปรเเกรมจะทำการเเปลงภาษา HTML ซึ่งเป็นภาษาที่นิยมใช้ในการพัฒนาเว็บ ให้เป็นภาษาที่คนทั่วไปสามารถเห็นหรือเข้าใจได้บนหน้าเว็บเพจ (Web Page)

![Untitled](https://etutorials.org/shared/images/tutorials/tutorial_78/process_.jpg)

_ภาพจาก :_ [https://etutorials.org/shared/images/tutorials/tutorial*78/process*.jpg](https://etutorials.org/shared/images/tutorials/tutorial_78/process_.jpg)

โดยการทำงานของเว็บบราวเซอร์นั้น การเข้าชมเว็บไซต์ผู้ใช้ต้องกรอกสิ่งที่เรียกว่า URL หรือ Web Address เช่น [www.google.com](http://www.google.com) หรือ [www.facebook.com](http://www.facebook.com) ลงไป ตัวเว็บบราวเซอร์ก็จะทำงานส่งคำร้อง (Request) ไปที่เว็บเซิฟเวอร์ (Web Server) ของเว็บไซต์นั้น ๆ จากนั้นตัวเว็บเซิฟเวอร์ (Web Server) ก็จะทำการส่งข้อมูลของเว็บไซต์นั้น ๆ ที่อยู่ในรูปของไฟล์ HTML (Hypertext Markup Langauge) มายังเว็บบราวเซอร์ โดยผ่าน Hypertext Transfer Protocol (HTTP) จากนั้นตัวเว็บบราวเซอร์ก็จะทำการประมวลผลข้อมูล เเละเเสดงข้อมูลบนหน้าเว็บเพจกลับไปยังผู้ใช้

### วิธีการติดตั้ง Chrome Web Browser บน Ubuntu Linux โดยใช้ CLI

การติดตั้ง Google Chrome บน Ubuntu Linux สามารถทำได้โดยใช้ Built-it Package Manager ที่ติดมากับ Ubuntu Linux อย่าง APT (Advanced Package Tool) โดย APT นอกจากจะใช้ในการติดตั้งซอฟต์เเวร์เเล้ว ยังสามารถใช้ในการจัดการ ตั้งค่าเเพ็กเก็จต่าง ๆ ได้อีกด้วย

โดยซอฟต์แวร์ที่ติดตั้งโดยใช้ APT จะถูกเก็บในโฟลเดอร์ที่ชื่อว่า `/etc/apt/sources.list` ซึ่งใช้สำหรับเก็บข้อมูลต่าง ๆ ของเเพ็กเก็จ (Repository) ที่ Ubuntu Linux ใช้สำหรับติดตั้งและอัพเดทเเพ็กเก็จ

ตัวอย่างคำสั่งของ APT ที่น่าสนใจเเละมักจะถูกใช้บ่อย

- `apt-get install [ชื่อแพ็คเกจ]` ติดตั้งแพ็กเกจและ dependency ทั้งหมดรวมทั้งแพ็กเกจที่แนะนำตามค่าเริ่มต้น
- `apt-get remove [ชื่อแพ็คเกจ]` ลบแพ็กเกจที่มีอยู่และแพ็กเกจที่ขึ้นอยู่กับแพ็กเกจนี้ อย่างไรก็ตาม dependency ของแพ็กเกจหรือไฟล์ configuration จะไม่ถูกลบออก
- `apt-get --purge remove [ชื่อแพ็คเกจ]` ลบแพ็กเกจและไฟล์คอนฟิกูเรชัน
- `apt-get upgrade` อัพเกรดแพ็กเกจทั้งหมดหากเป็นไปได้ แต่ไม่ติดตั้งแพ็กเกจใหม่ (ซึ่งบางเวลาอาจจำเป็นเพื่อให้ระบบทันสมัยเพราะมี dependency ที่เปลี่ยนไป)
- `apt-get dist-upgrade` อัพเกรดแพ็กเกจทั้งหมดให้ทันสมัย และติดตั้งแพ็กเกจใหม่หากจำเป็น หรือลบแพ็กเกจที่ขัดแย้งกับแพ็กเกจที่กำลังติดตั้ง
- `apt-get update` รับข้อมูลล่าสุดของแพ็คเกจจากเซิร์ฟเวอร์ของเดเบียน
- `apt-get source [ชื่อแพ็คเกจ]` ดึงซอร์สโค้ดของแพ็กเกจจากเซิร์ฟเวอร์ของเดเบียนไปยัง directory ปัจจุบัน
- `apt-cache search [คำค้นหา]` ค้นหาแพ็กเกจ

**Step 01: ทำการอัพเดท Ubuntu Linux เเพ็กเก็จให้เป็นเวอร์ชั่นล่าสุดโดยใช้ APT**

โดยสองคำสั่งนี้จะใช้ในการอัพเดทระบบ รวมถึงเเพ็กเก็จต่าง ๆ (System Repositories) ที่ติดตั้งเอาไว้ก่อนหน้านี้ให้เป็นเวอร์ชั่นล่าสุด

```bash
sudo apt update && sudo apt upgrade
```

![Untitled](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-04%20at%2019.37.27.png?raw=true)

**Step 02: ติดตั้ง Packages ที่จำเป็นสำหรับการใช้งาน Google Chrome บน Ubuntu Linux**

ในการติดตั้ง Google Chrome บน Ubuntu Linux จำเป็นต้องใช้ Package อื่น ๆ ที่จำเป็นในการใช้งาน ดังนั้นก่อนการติดตั้งเเละใช้งาน Google Chrome เราจึงจำเป็นต้องติดตั้ง Package อื่น ๆ ที่จำเป็น ประกอบไปด้วย

- **software-properties-common** จัดเตรียมเครื่องมือและไลบรารีสำหรับการจัดการกับ software repositories บน Ubuntu
- **apt-transport-https** ทำให้การติดตั้ง Package ผ่าน APT รองรับการทำงานบนโปรโตคอลเเบบ HTTPS
- **ca-certificates** ทำให้การเชื่อมต่อไปยัง Repository ผ่าน HTTPS มีการใช้งานควบคู่กับใบรับรอง CA

```bash
sudo apt install curl software-properties-common apt-transport-https
ca-certificates -y
```

![Untitled](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-04%20at%2019.39.25.png?raw=true)

**Step 03: ทำการ Import Google Chrome APT Repository บน Ubuntu**

ก่อนการติดตั้ง Google Chrome นั้น เพื่อทำการดาวน์โหลดหรือติดต่อกับ Google Chrome Repository เราจำเป็นจะต้อง Import ตัว GPG Key มาก่อน

```bash
curl -fSsL <https://dl.google.com/linux/linux_signing_key.pub> | gpg --dearmor |
sudo tee /usr/share/keyrings/google-chrome.gpg > /dev/null
```

```bash
echo deb [arch=amd64 signed-by=/usr/share/keyrings/google-chrome.gpg]
<http://dl.google.com/linux/chrome/deb/> stable main |
sudo tee /etc/apt/sources.list.d/google-chrome.list
```

![Untitled](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-04%20at%2019.40.25.png?raw=true)

**Step 04: ทำการอัพเดท APT Cache หลังจาก Import Google Chrome Repository**

```bash
sudo apt update
```

**Step 05: ทำการติดตั้ง Goole Chrome**

หลังจากที่เราผ่าน Step 01 - Step 04 มาเเล้วนั้น ตอนนี้ก็สามารถที่จะติดตั้ง Google Chrom ผ่าน APT ได้เเล้ว โดยการใช้คำสั่ง

```bash
sudo apt install google-chrome-stable
```

![Untitled](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-04%20at%2019.41.14.png?raw=true)

นอกจากคำสั่งนี้เเล้ว เรายังสามารถติดตั้ง Google Chrome Edition อื่น ๆ ได้อีกด้วย ไม่ว่าจะเป็น

- Google Chrome Beta: `sudo apt install google-chrome-beta`
- Google Chrome Unstable: `sudo apt install google-chrome-unstable`

เพียงเท่านี้ถ้าเราลองไปดูใน Apps Library บน Ubuntu เราก็จะเห็นว่ามี Google Chrome ขึ้นมาให้เราสามารถใช้งานได้เเล้ว

![Untitled](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-04%20at%2019.41.31.png?raw=true)

![Untitled](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-04%20at%2019.41.46.png?raw=true)

## 2. เว็บเซิฟเวอร์ (Web Server)

คอมพิวเตอร์ที่ทำการติดตั้งซอฟต์เเวร์หรือโปรเเกรมที่ใช้สำหรับโต้ตอบกับผู้ใช้เมื่อมีการส่ง Request เข้ามา รวมถึงยังเป็นที่เก็บไฟล์ต่าง ๆ ที่เกี่ยวข้องกับเว็บไซต์ เช่น HTML CSS, Image และ JavaScript เป็นต้น โดยเว็บเซิร์ฟเวอร์ทำหน้าที่ส่งหน้าเว็บไปยังผู้ใช้ (Client) ตามคำขอ (Request) ของผู้ใช้ผ่านเว็บเบราว์เซอร์ที่เราใช้กัน เช่น Google Chrome, Firefox, Safari เป็นต้น

![Untitled](https://devhub.in.th/media/django-summernote/2023-04-10/f1d051d1-72c7-4a40-9f5e-69283fa9330a.jpg)

ภาพจาก: [https://devhub.in.th/media/django-summernote/2023-04-10/f1d051d1-72c7-4a40-9f5e-69283fa9330a.jpg](https://devhub.in.th/media/django-summernote/2023-04-10/f1d051d1-72c7-4a40-9f5e-69283fa9330a.jpg)

### วิธีการติดตั้งเเละใช้งาน Apache Web Server บน Ubuntu Linux

การติดตั้งเเละใช้งาน Web Server บน Linux นั้น เราจะใช้โปรเเกรมที่ชื่อว่า XAMPP ที่ย่อมากจาก cross-platform(X), Apache(A) server, MariaDB(M), PHP(P), and Perl(P) ถูกพัฒนาโดย Apache Friends เป็นโปรเเกรมที่ฟรี เเละ Open Source สำหรับการทำ Web Server

**Step 01: ทำการดาวน์โหลด XAMPP Installation Package**

สำหรับการดาวน์โหลด XAMPP นั้นเราสามารถเข้าไปที่หน้าเว็บ [https://www.apachefriends.org/index.html](https://www.apachefriends.org/index.html) เเละเราก็เลือกไปที่ XAMPP for Linux เพราะเราจะมาติดตั้งบน Ubuntu Linux นั้นเอง

![Untitled](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-04%20at%2020.11.38.png?raw=true)

**Step 02: ทำให้ Installation Package ที่เราดาวน์โหลดมาสามารถ Execute ได้**

โดยปกติ Installer ที่เราดาวน์โหลดมานั้นจะยังไม่สามารถรันหรือ Execute ได้ เนื่องจากยังไม่มี Permission ในการ Execute นั้นเอง เราเลยต้องมีการใช้คำสั่งในการทำให้ XAMPP Installer นั้นสามารถที่จะรันเเละติดตั้งได้

1.  **ทำการเปิด Terminal เเละ cd ไปที่ /downloads**

```bash
$ cd /home/[username]/Downloads
```

2.  **เรียกใช้คำสั่ง chmod สำหรับเเก้ไข Permission ของไฟล์ Installer**

```bash
$ chmod 755 xampp-linux-*-installer.run
```

![Screenshot 2567-02-04 at 20.33.47.png](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-04%20at%2020.33.47.png?raw=true)

ถ้าเราลองใช้คำสั่ง ls -l เพื่อดู Permission ของไฟล์ก็จะพบว่า XAMPP Installer นั้นมี Permission `rwxr` ที่สามารถถูกเรียกหรือ Execute โดย User ได้เเล้ว เพียงเท่านี้ถ้าเราลองรันไฟล์ XAMPP Installer ก็จะสามารถรันเเละติดตั้ง XAMPP ลงในเครื่องของเราได้เเล้ว

![Untitled](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-04%20at%2020.33.58.png?raw=true)

**Step 03: ทำการเรียกใช้งาน XAMPP Installer**

ในขั้นตอนนี้เราก็จะมารัน XAMPP Installer เพื่อทำการติดตั้ง XAMPP โดยใช้คำสั่ง

```bash
$ sudo ./[package name]
```

จากนั้นก็ทำการติดตั้ง XAMPP ผ่าน Setup WIzard ได้ตามขั้นตอนที่ขึ้นบนหน้าจอเลย
![Untitled](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-05%20at%2001.00.34.png?raw=true)

**Step 04: เรียกใช้ XAMPP เเละ Start Services**

จากนั้นเมื่อติดตั้ง XAMPP สำเร็จ เราสามารถเรียกใช้ XAMPP Control Panel ได้โดยใช้คำสั่ง

(ในการใช้งานครั้งเเรกจำเป็นต้องติดตั้ง net-tools ซึ่งเป็นเป็นแพ็กเกจซอฟต์แวร์สำหรับระบบปฏิบัติการ Linux ที่ประกอบไปด้วยชุดโปรแกรมสำหรับการจัดการเครือข่าย)

```bash
sudo apt install net-tools
```

```bash
sudo /opt/lampp/lampp start
```

![Screenshot 2567-02-04 at 20.43.17.png](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-05%20at%2001.00.13.png?raw=true)

หลังจากนั้นถ้าเราลองเปิด Web Browser เเละเข้าไปที่ [http://localhost](http://localhost) เราก็จะพบว่ามีหน้าเว็บของ XAMPP ที่เป็น Web Server มาเเสดงผลให้เราได้เห็นเเล้ว

![Screenshot 2567-02-04 at 20.43.37.png](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-05%20at%2001.02.31.png?raw=true)

**Step 05: ปิดการใช้งาน XAMPP**

เมื่อเลือกใช้งานเเล้ว เราสามารถปิดหรือหยุดการทำงานของ XAMPP ได้โดยใช้คำสั่ง

```bash
sudo /opt/lampp/lampp stop
```

![Screenshot 2567-02-04 at 20.44.19.png](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-05%20at%2001.03.07.png?raw=true)

จากนั้นเมื่อเราลองกลับไปที่ [http://localhost](http://localhost) ก็จะพบว่าไม่สามารถเข้าหน้าเว็บได้เเล้ว เนื่องจากเราทำการปิด Web Server ไปเเล้วนั้นเอง

![Screenshot 2567-02-04 at 20.44.34.png](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/Screenshot%202567-02-05%20at%2001.04.27.png?raw=true)

## 3. ภาษาเขียนโปรเเกรม (Programming Language)

ภาษาเขียนโปรแกรม (Programming Language) เปรียบเสมือนภาษาที่ใช้สื่อสารกับคอมพิวเตอร์ ช่วยให้มนุษย์สามารถสั่งให้คอมพิวเตอร์ทำงานตามต้องการ โดยใช้ชุดคำสั่ง (Instructions) และไวยากรณ์ (Syntax) ที่เฉพาะเจาะจง ภาษาเขียนโปรแกรมมีหลากหลายประเภท แต่ละภาษาถูกออกแบบมาเพื่อการใช้งานในลักษณะที่แตกต่างกัน

ภาษาเขียนโปรแกรมที่มักจะถูกใช้สำหรับการพัฒนาเว็บไซต์ก็มีหลายภาษา ไม่ว่าจะเป็น HTML, CSS, JavaScirpt เเละ PHP โดยหน้าที่ของแต่ละภาษาก็แบ่งได้เป็น

**1. HTML:** ภาษาที่ใช้สร้างโครงสร้างพื้นฐานของหน้าเว็บ กำหนดส่วนต่างๆ ของหน้าเว็บ เช่น หัวข้อ เนื้อหา รูปภาพ วิดีโอ

**2. CSS:** ภาษาที่ใช้ควบคุมสไตล์ของหน้าเว็บ กำหนดสี รูปแบบ ตัวอักษร ตำแหน่งขององค์ประกอบต่างๆ บนหน้าเว็บ

**3. JavaScript:** ภาษาที่ใช้เพิ่มการโต้ตอบบนหน้าเว็บ ทำให้หน้าเว็บมีชีวิตชีวา ตอบสนองต่อผู้ใช้ เช่น แสดงข้อความแจ้งเตือน ตรวจสอบความถูกต้องของข้อมูล

### ตัวอย่างการใช้ภาษา HTML สำหรับพัฒนาเว็บไซต์

HTML หรือ Hyper Text Markup Language เป็นภาษาประเภท Markup Language ที่ใช้ในการสร้างเว็บเพจ มีแม่แบบมาจากภาษา SGML (Standard Generalized Markup Language) ที่ตัดความสามารถบางส่วนออกไป เพื่อให้สามารถทำความเข้าใจและเรียนรู้ได้ง่าย ปัจจุบันมีการพัฒนาและกำหนดมาตรฐานโดยองค์กร World Wide Web Consortium (W3C)

ภาษา HTML มีโครงสร้างการเขียนโดยอาศัย **Tag** ในการควบคุมการแสดงผลของข้อความ รูปภาพ หรือวัตถุอื่น ๆ แต่ละ Tag อาจจะมีส่วนขยาย เรียกว่า **Attribute** สําหรับจัดรูปแบบเพิ่มเติม

**รูปเเบบของภาษา HTML ที่ประกอบด้วย Tag เเละ Attributes**

```html
<tag attribute1="value1" attribute2="value2">''content''</tag>
```

**HTML Tags อื่น ๆ ที่น่าสนใจ และมักจะถูกใช้ในการพัฒนาเว็บ**

- **แท็กโครงสร้าง (Structural tags):**
  - `<html>`: กำหนดจุดเริ่มต้นและจุดสิ้นสุดของเอกสาร HTML
  - `<head>`: เก็บข้อมูลเกี่ยวกับเอกสาร HTML เช่น หัวเรื่อง คำอธิบาย
  - `<body>`: เก็บเนื้อหาหลักของเว็บไซต์
  - `<h1>` ถึง `<h6>`: กำหนดขนาดหัวเรื่อง
  - `<p>`: กำหนดย่อหน้า
  - `<br>`: ขึ้นบรรทัดใหม่
- **แท็กการจัดรูปแบบ (Formatting tags):**
  - `<b>`: เน้นข้อความ
  - `<i>`: เอียงข้อความ
  - `<pre>`: แสดงข้อความแบบคงรูปแบบ
  - `<hr>`: ขีดเส้นแบ่ง
- **แท็กการเชื่อมโยง (Linking tags):**
  - `<a>`: แทรกการเชื่อมโยงไปยังเว็บไซต์อื่น
- **แท็กภาพ (Image tags):**
  - `<img>`: แสดงรูปภาพ
- **แท็กตาราง (Table tags):**
  - `<table>`: กำหนดตาราง
  - `<tr>`: กำหนดแถว
  - `<td>`: กำหนดเซลล์
- **แท็กวิดีโอ (Video tags):**
  - `<video>`: แสดงวิดีโอ
- **แท็กแบบฟอร์ม (Form tags):**
  - `<form>`: กำหนดแบบฟอร์ม
  - `<input>`: กำหนดช่องป้อนข้อมูล
  - `<button>`: กำหนดปุ่ม

**ตัวอย่างการใช้ภาษา HTML สำหรับสร้างหน้าเว็บ เเละเเสดงข้อความ “Hello Web” เบื้องต้น**

```html
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Lab 1</title>
  </head>
  <body>
    <h1>Hello Web !!!</h1>
  </body>
</html>
```

![Screenshot 2567-02-04 at 23.04.07.png](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-04%20at%2023.31.17.png?raw=true)

### ตัวอย่างการใช้ภาษา CSS สำหรับพัฒนาเว็บไซต์

CSS ย่อมาจาก Cascading Style Sheets เป็นภาษาที่ใช้ควบคุมรูปแบบของหน้าเว็บ ช่วยให้สามารถกำหนดสี ตัวอักษร ขนาด รูปแบบ และตำแหน่งขององค์ประกอบต่างๆ บนหน้าเว็บ CSS ประกอบด้วย 3 รูปแบบหลัก ดังนี้

1.  **Inline CSS** (การเขียน CSS ลงไปใน HTML Tag)

```html
<p style="color: red; font-size: 18px;">Sila Pakdeewong</p>
```

1.  **Embedded CSS** (การเขียน CSS ลงไปในส่วนของ HTML Head)

```html
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Lab 1</title>

    <style>
      body {
        font-family: "Nunito", sans-serif;
        background-color: #f6ddcc;
        text-align: center;
      }
    </style>
  </head>

  <body>
    <h1>Hello Web !!!</h1>
  </body>
</html>
```

1.  **External CSS** (การเขียน CSS นอกไฟล์ HTML และลิงค์มายังไฟล์ HTML)

- **ไฟล์ style.css**

```css
body {
  color: #000;
  font-family: Arial, sans-serif;
}

h1 {
  font-size: 2em;
  text-align: center;
}

p {
  margin: 1em;
}
```

- **ไฟล์ index.html**

```html
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Lab 1</title>

    <link rel="stylesheet" href="style.css" />
  </head>

  <body>
    <h1>Hello Web !!!</h1>
  </body>
</html>
```

### ตัวอย่างการใช้ภาษา JavaScript สำหรับพัฒนาเว็บไซต์

JS หรือ JavaScript เป็นหนึ่งในภาษาเขียนโปรแกรมที่นิยมใช้ในการพัฒนาเว็บไซต์ โดยมีจุดประสงค์เพื่อเอาไว้จัดการพฤติกรรมต่าง ๆ ที่เกิดขึ้นจากผู้ใช้งาน บนหน้าเว็บไซต์ในฝั่งของ Client นอกจากนี้ในบางเฟรมเวิร์คภาษา JavaScript ยังถูกใช้ในการพัฒนาฝั่ง Server อีกด้วย

**ฟังก์ชันภาษา JavaScript ที่มักจะถูกใช้ในการพัฒนาเว็บ**

**ฟังก์ชันพื้นฐาน:**

- `alert()`: แสดงข้อความแจ้งเตือน
- `confirm()`: แสดงข้อความแจ้งเตือนพร้อมปุ่มยืนยันและยกเลิก
- `prompt()`: แสดงข้อความแจ้งเตือนพร้อมช่องป้อนข้อมูล
- `console.log()`: แสดงข้อความบนคอนโซล
- `document.getElementById()`: ค้นหาองค์ประกอบ HTML โดย ID
- `document.getElementsByClassName()`: ค้นหาองค์ประกอบ HTML โดย class
- `document.querySelector()`: ค้นหาองค์ประกอบ HTML โดย selector

**ฟังก์ชันสำหรับการจัดการ DOM:**

- `innerHTML`: ตั้งค่าเนื้อหา HTML ลงไปใน Element
- `outerHTML`: ตั้งค่าเนื้อหา HTML ทั้งหมดของ Element
- `appendChild()`: เพิ่ม HTML Element ลงไปใน Element เดิม
- `removeChild()`: ลบ HTML Element ออกจาก Element เดิม
- `insertBefore()`: แทรก HTML Element ก่อนหน้า Element เดิม
- `replaceChild()`: แทนที่ HTML Element ด้วย Element อื่น ๆ

**ฟังก์ชันสำหรับการจัดการเหตุการณ์:**

- `addEventListener()`: เพิ่ม event listener ให้กับ HTML Element
- `removeEventListener()`: ลบ event listener ออกจาก HTML Element
- `preventDefault()`: ยับยั้งการดำเนินการเริ่มต้นของเหตุการณ์
- `stopPropagation()`: หยุดการ propagate ของเหตุการณ์

**ฟังก์ชันสำหรับการจัดการเวลา:**

- `setTimeout()`: ตั้งเวลา setTimeout
- `setInterval()`: ตั้งเวลา setInterval
- `clearTimeout()`: ล้าง setTimeout
- `clearInterval()`: ล้าง setInterval

**ฟังก์ชันสำหรับการจัดการข้อมูล:**

- `parseInt()`: แปลง string เป็น integer
- `parseFloat()`: แปลง string เป็น float
- `isNaN()`: ตรวจสอบว่าค่าเป็น NaN หรือไม่
- `Math.random()`: สุ่มเลขจำนวนเต็ม

**ฟังก์ชันสำหรับการจัดการ Array:**

- `Array.prototype.push()`: เพิ่ม element ลงท้าย array
- `Array.prototype.pop()`: ลบ element สุดท้ายออกจาก array
- `Array.prototype.unshift()`: เพิ่ม element ลงหน้า array
- `Array.prototype.shift()`: ลบ element แรกออกจาก array
- `Array.prototype.slice()`: คัดลอกส่วนหนึ่งของ array
- `Array.prototype.join()`: แปลง array เป็น string

**ฟังก์ชันสำหรับการจัดการ Object:**

- `Object.keys()`: ดึง key ทั้งหมดของ object
- `Object.values()`: ดึง value ทั้งหมดของ object

**ตัวอย่างวิธีการใช้งานภาษา JavaScript**

1.  **Inline JavaScript** (การเขียนภาษา JavaScript ลงไปใน HTML Tag)

```html
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Lab 1</title>
  </head>
  <body>
    <h1>Hello Web !!!</h1>
    <button id="my-button" onclick="alert('Button has been clicked!')">Click Me</button>
  </body>
</html>
```

1.  **Embedded JavaScript** (การเขียนภาษา JavaScript ลงไปใน ไฟล์ HTML)

```html
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Lab 1</title>
  </head>
  <body>
    <h1>Hello Web !!!</h1>
    <button id="my-button">Click Me</button>

    <script>
      const button = document.getElementById("my-button");

      button.addEventListener("click", () => {
        alert("Button has been clicked!");
      });
    </script>
  </body>
</html>
```

1.  **External JavaScript** (การเขียนภาษา JavaScript เเละลิงค์มายังไฟล์ HTML)

- **ไฟล์ index.js**

```jsx
const button = document.getElementById("my-button");

button.addEventListener("click", () => {
  alert("Button has been clicked!");
});
```

- **ไฟล์ index.html**

```html
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Lab 1</title>
  </head>
  <body>
    <h1>Hello Web !!!</h1>
    <button id="my-button">Click Me</button>

    <script src="index.js"></script>
  </body>
</html>
```

จากโค๊ดตัวอย่าง ทั้ง 3 วิธีเป็นการเรียกใช้งานภาษา JavaScript ให้ทำการเเสดง Alert เเก่ผู้ใช้เมื่อทำการกดปุ่มภายในหน้าเว็บ

![Screenshot 2567-02-04 at 23.31.17.png](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-04%20at%2023.32.01.png?raw=true)

### การทำงานของภาษา JavaScript บน Web Browser โดยใช้ JavaScript Engine

![Untitled](https://res.cloudinary.com/practicaldev/image/fetch/s--hDrS3fyq--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/baivubsmprmukfu2jyqc.png)

รูปภาพจาก [https://dev.to/varunprashar5/how-javascript-engine-s-work-3cb0](https://dev.to/varunprashar5/how-javascript-engine-s-work-3cb0)

ภาษา JavaScript ถูกเรียกใช้บน Web Browser ผ่านกลไก JavaScript Engine ที่ฝังอยู่ในตัว Browser เอง กลไกนี้ทำหน้าที่แปลโค้ด JavaScript ให้เป็นภาษาที่เครื่องเข้าใจและสามารถทำงานได้

**ขั้นตอนการทำงานของ JavaScript Engine:**

1.  **การแปลโค้ด (Parsing):** JavaScript Engine จะวิเคราะห์ไวยากรณ์ของโค้ด JavaScript และแปลงเป็นรูปแบบ Abstract Syntax Tree (AST) ซึ่งเป็นโครงสร้างข้อมูลที่แสดงความสัมพันธ์ของส่วนต่างๆ ของโค้ด
2.  **การรวบรวมขยะ (Garbage Collection):** JavaScript Engine จะจัดการหน่วยความจำที่ใช้โดยโค้ด JavaScript เก็บขยะหน่วยความจำที่ไม่ใช้งานเพื่อป้องกันปัญหาด้านหน่วยความจำ
3.  **การประมวลผล JIT (Just-In-Time Compilation):** JavaScript Engine จะแปลงโค้ด JavaScript บางส่วนให้เป็นภาษาเครื่องโดยตรงก่อนรัน ช่วยให้รันโค้ดได้เร็วขึ้น
4.  **การรันโค้ด (Execution):** JavaScript Engine จะรันโค้ด JavaScript ที่แปลแล้วบน CPU

**ประเภทของ JavaScript Engine:**

- **V8:** พัฒนาโดย Google เป็น JavaScript Engine ที่ใช้ใน Chrome, Opera และ Edge
- **SpiderMonkey:** พัฒนาโดย Mozilla เป็น JavaScript Engine ที่ใช้ใน Firefox
- **JavaScriptCore:** พัฒนาโดย Apple เป็น JavaScript Engine ที่ใช้ใน Safari

## 4. โปรเเกรมสำหรับเขียนโค๊ด (Integrated Development Environment)

![Untitled](https://d1.awsstatic.com/whatisimg/C9-Collab-Image%403x.e03a65d9488633c154358430540ab363dd1e8f45.b0e71758c4bd505e525f90e0ff8db5859a82397a.png)

รูปภาพประกอบจาก [https://aws.amazon.com/th/what-is/ide/](https://aws.amazon.com/th/what-is/ide/)

IDE หรือ Integrated Development Environment เป็นโปรเเกรมที่รวบรวมเอาชุดเครื่องมือเเละคุณสมบัติต่าง ๆ ที่ต้องใช้ในการพัฒนาซอฟต์เเวร์มาอยู่ในโปรเเกรมเฉพาะสำหรับนักพัฒนาซอฟต์เเวร์ โดยจะนำส่วนประกอบของเครื่องมือต่างๆมารวมกันเช่น Code Editor, การ Compiler หรือ Interpreter, Debugger เป็นต้น

**IDE ยอดนิยม เเละถูกเลือกใช้ในการพัฒนาโปรเเกรมภาษาต่าง ๆ**

- **Visual Studio:** พัฒนาโดย Microsoft รองรับภาษาโปรแกรมหลายภาษา เช่น C++, C#, Visual Basic
- **Eclipse:** พัฒนาโดย Eclipse Foundation เป็น open-source IDE รองรับภาษาโปรแกรมหลายภาษา เช่น Java, C++, PHP
- **IntelliJ IDEA:** พัฒนาโดย JetBrains รองรับภาษาโปรแกรมหลายภาษา เช่น Java, Kotlin, Python
- **WebStorm:** พัฒนาโดย JetBrains รองรับภาษา JavaScript และ TypeScript

### วิธีการติดตั้งเเละใช้งาน Visual Studio Code บน Ubuntu Linux

**Visual Studio Code (VS Code)** เป็นโปรแกรม Text Editor ที่ใช้สำหรับการเขียนโปรเเกรม สร้างโดย Microsoft เหมาะสำหรับการเขียน และ Debug ภาษาโปรแกรมหลากหลายภาษา นิยมใช้ในการพัฒนาเว็บ และได้รับความนิยมอย่างมากจากนักพัฒนาทั่วโลก ด้วยคุณสมบัติเด่น ดังนี้:

- **รองรับหลายภาษา:** VS Code สนับสนุนภาษาโปรแกรมยอดนิยม เช่น JavaScript, Python, C++, C#, Java, PHP, Go, และอื่นๆ อีกมาก
- **ส่วนขยาย:** ขยายฟังก์ชันการทำงานได้ เพิ่มเติมฟีเจอร์ต่างๆ ตามความต้องการ เช่น code snippets, debugging tools, linters, themes, และอื่นๆ
- **ปรับแต่งได้:** ปรับแต่งธีม, แป้นพิมพ์ลัด และการตั้งค่าต่างๆ เพื่อให้ใช้งานได้สะดวก
- **Git และ GitHub:** มีการควบคุม Git ในตัว เชื่อมต่อกับ GitHub ได้สะดวก
- **ดีบักกิ้ง:** ดีบักโค้ดได้สะดวก มีเครื่องมือดีบักกิ้งในตัว
- **เบาและรวดเร็ว:** ใช้ทรัพยากรระบบน้อย ใช้งานได้รวดเร็ว
- **โอเพนซอร์ส:** ฟรีและมีชุมชนนักพัฒนาขนาดใหญ่ สนับสนุนและพัฒนาต่อเนื่อง

ในการติดตั้ง Visual Studio Code บน Linux นั้น เราสามารถใช้ Package Manager ชื่อชื่อว่า Snap ซึ่งเป็น Package Manager ที่ Built-in มาใน Ubuntu Linux นอกเหนือจาก APT มาใช้ในการติดตั้ง Package หรือซอฟต์เเวร์อื่น ๆ ที่ต้องการได้

**ตัวอย่างคำสั่งของ Snap ที่ใช้ในการจัดการ Package หรือเเอปพลิเคชัน**

- **ติดตั้งแอปพลิเคชัน:** `sudo snap install <ชื่อแอปพลิเคชัน>`
- **ค้นหาแอปพลิเคชัน:** `snap find <ชื่อแอปพลิเคชัน>`
- **ดูรายการแอปพลิเคชันที่ติดตั้ง:** `snap list`
- **อัปเดตแอปพลิเคชัน:** `sudo snap refresh <ชื่อแอปพลิเคชัน>`
- **ลบแอปพลิเคชัน:** `sudo snap remove <ชื่อแอปพลิเคชัน>`

**Step 01: ติดตั้ง VS Code โดยใช้ Snap**

```bash
sudo snap install --classic code
```

![Screenshot 2567-02-04 at 23.57.50.png](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-04%20at%2023.57.50.png?raw=true)

**Step 02: หลังจาก Snap ทำการติดตั้ง VS Code เสร็จ เราสามารถเช็ค Version ของ VS Code ได้ โดยใช้**

```bash
code --version
```

![Screenshot 2567-02-05 at 00.01.33.png](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-05%20at%2000.01.33.png?raw=true)

เพียงเท่านี้เราก็จะได้ Visual Studio Code ซึ่งเป็น IDE ที่พัฒนาโดย Microsoft เเละยังสามารถติดตั้งส่วนเสริมที่รองรับหลายภาษาเขียนโปรเเกรม มาใช้งานเเล้ว

![Screenshot 2567-02-05 at 00.03.44.png](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-05%20at%2000.03.44.png?raw=true)

## ตัวอย่างการพัฒนาเว็บโดยใช้ภาษา HTML CSS JavaScript ร่วมกับ Apache Web Server บน Ubuntu Linux

**Step 01: ทำการเข้าไปในโฟลเดอร์ htdocs ของ XAMPP Web Server**

โดยโฟลเดอร์ htdocs นี้โดยปกติ Xampp จะทำการใช้โฟเดอร์นี้ในการเก็บ Directory ต่าง ๆ ของเว็บ โดยจะสังเกตุว่าโดยปกติถ้าเราเข้า [http://localhost](http://localhost) ตัวเว็บจะถูก redirect ไปที่ [http://localhost/dashboard](http://localhost/dashboard) ซึ่งถ้าเราลองไปดูในโฟลเดอร์ htdocs ก็จะเห็นว่า มี directory ที่ชื่อว่า /dashbaord อยู่ เเละ ในนั้นประกอบไปด้วยไฟล์ของหน้านั้น ๆ

![Screenshot 2567-02-05 at 00.39.52.png](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-05%20at%2000.39.52.png?raw=true)

**Step 02: สร้าง Directory สำหรับเก็บไฟล์เอกสาร Web**

เนื่องจากในการพัฒนาเว็บไซต์จะต้องมีการใช้ไฟล์ HTML CSS เเละ JavaScript ดังนั้น เราจึงต้องสร้าง Directory สำหรับเก็บไฟล์ทั้ง 3 อันนี้ ในที่นี้จะใช้ชื่อว่า `webprog` ภายใน `htdocs` การทำเเบบนี้จะทำให้เราสามารถเปิดเว็บได้โดยใช้ [http://localhost/webprog](http://localhost/webprog)

```bash
mkdir webprog
```

**Step 03: ทำการสร้างไฟล์ index.html index.js เเละ style.css**

ในขั้นตอนนี้เราจะมาสร้างไฟล์ที่ใช้สำหรับเว็บ โดยประกอบไปด้วย

1.  **index.html** สำหรับเก็บโครงสร้าง เเละ HTML Elements ต่างๆ ของหน้าเว็บ

![Untitled](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-05%20at%2000.31.30.png?raw=true)

1.  **index.js** สำหรับกำหนดพฤติกรรมต่าง ๆ ให้กับ HTML Elements

![Untitled](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-05%20at%2000.32.10.png?raw=trueg)

1.  **style.css** สำหรับกำหนดรูปร่าง สไตล์ให้กับ HTML Elements

![Untitled](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-05%20at%2000.31.52.png?raw=true)

**Step 04: จากนั้นทำการลองเข้าเว็บไซต์ที่เราสร้างขึ้นมา**

เนื่องจากเราเก็บไฟล์ของเว็บทั้งหมดเอาไว้ที่ `/htdocs/webprog` ทำให้เราสามารถเข้าเว็บที่พึ่งสร้างเอวไว้ผ่าน [http://localhost/webprog](http://localhost/webprog) ได้เลย

หลังจากนั้นเมื่อเข้ามาก็จะเจอกับหน้าเว็บที่เราพึ่งสร้างนั้นเอง โดยจะประกอบไปด้วยข้อความ เเละปุ่มให้ผู้ใช้กด

![Screenshot 2567-02-05 at 00.33.15.png](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-05%20at%2000.33.15.png?raw=true)

เมื่อผู้ใช้กดปุ่ม เว็บก็จะขึ้นหน้าต่างมาถามชื่อ หลังจาดนั้นเมื่อกรอกชื่อก็จะทำการขึ้นข้อความ Hello, welcome back ตามด้วยชื่อที่เราใส่ไป

![Screenshot 2567-02-05 at 00.33.11.png](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-05%20at%2000.33.11.png?raw=true)

![Screenshot 2567-02-05 at 00.33.14.png](https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Screenshot%202567-02-05%20at%2000.33.14.png?raw=true)

## References

1.  [https://en.wikipedia.org/wiki/Web_development_tools](https://en.wikipedia.org/wiki/Web_development_tools)
2.  [](<https://th.wikipedia.org/wiki/%E0%B9%80%E0%B8%AD%E0%B8%9E%E0%B8%B5%E0%B8%97%E0%B8%B5_(%E0%B8%8B%E0%B8%AD%E0%B8%9F%E0%B8%95%E0%B9%8C%E0%B9%81%E0%B8%A7%E0%B8%A3%E0%B9%8C)>)[https://th.wikipedia.org/wiki/เอพีที\_(ซอฟต์แวร์)](<https://th.wikipedia.org/wiki/%E0%B9%80%E0%B8%AD%E0%B8%9E%E0%B8%B5%E0%B8%97%E0%B8%B5_(%E0%B8%8B%E0%B8%AD%E0%B8%9F%E0%B8%95%E0%B9%8C%E0%B9%81%E0%B8%A7%E0%B8%A3%E0%B9%8C)>)
3.  [https://devhub.in.th/blog/what-is-web-server](https://devhub.in.th/blog/what-is-web-server)
4.  [](https://www.itgenius.co.th/article/%E0%B9%80%E0%B8%84%E0%B8%A3%E0%B8%B7%E0%B9%88%E0%B8%AD%E0%B8%87%E0%B8%A1%E0%B8%B7%E0%B8%AD%E0%B8%97%E0%B8%B5%E0%B9%88%E0%B9%83%E0%B8%8A%E0%B9%89%E0%B9%83%E0%B8%99%E0%B8%81%E0%B8%B2%E0%B8%A3%E0%B8%9E%E0%B8%B1%E0%B8%92%E0%B8%99%E0%B8%B2%E0%B9%80%E0%B8%A7%E0%B9%87%E0%B8%9A%E0%B9%84%E0%B8%8B%E0%B8%95%E0%B9%8C.html)[https://www.itgenius.co.th/article/เครื่องมือที่ใช้ในการพัฒนาเว็บไซต์.html](https://www.itgenius.co.th/article/%E0%B9%80%E0%B8%84%E0%B8%A3%E0%B8%B7%E0%B9%88%E0%B8%AD%E0%B8%87%E0%B8%A1%E0%B8%B7%E0%B8%AD%E0%B8%97%E0%B8%B5%E0%B9%88%E0%B9%83%E0%B8%8A%E0%B9%89%E0%B9%83%E0%B8%99%E0%B8%81%E0%B8%B2%E0%B8%A3%E0%B8%9E%E0%B8%B1%E0%B8%92%E0%B8%99%E0%B8%B2%E0%B9%80%E0%B8%A7%E0%B9%87%E0%B8%9A%E0%B9%84%E0%B8%8B%E0%B8%95%E0%B9%8C.html)
5.  [https://www.linuxcapable.com/install-google-chrome-on-ubuntu-linux/](https://www.linuxcapable.com/install-google-chrome-on-ubuntu-linux/)
6.  [https://thaibusinesssearch.com/marketing/web-browser/](https://thaibusinesssearch.com/marketing/web-browser/)
7.  [https://vitux.com/ubuntu-xampp/](https://vitux.com/ubuntu-xampp/)
8.  [https://en.wikipedia.org/wiki/HTML](https://en.wikipedia.org/wiki/HTML)
9.  [http://www.krukikz.com/index.php?option=com_content&view=article&id=119&Itemid=152](http://www.krukikz.com/index.php?option=com_content&view=article&id=119&Itemid=152)
10. [https://en.wikipedia.org/wiki/CSS](https://en.wikipedia.org/wiki/CSS)
11. [https://www.w3schools.com/js/](https://www.w3schools.com/js/)
12. [https://dev.to/varunprashar5/how-javascript-engine-s-work-3cb0](https://dev.to/varunprashar5/how-javascript-engine-s-work-3cb0)
13. [https://aws.amazon.com/th/what-is/ide/](https://aws.amazon.com/th/what-is/ide/)
