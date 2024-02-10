# Code Development Tools for Linux - (Group 02)

Linux ถือเป็นระบบปฎิบัติการหนึ่งที่มีความน่าสนใจ เเละความสามารถในการใช้งานด้านต่าง ๆ หนึ่งในการทำงานที่สำคัญ เเละเป็นที่นิยมในการใช้งานระบบปฎิบัติการ Linux นั้นก็คือการใช้งาน Code Development หรือการใช้งานระบบปฎิบัติการ Linux เพื่อพัฒนาโปรเเกรม เเอปพลิเคชั่นต่าง ๆ รวมถึงการพัฒนาเว็บ โดยผ่านการเขียนโค๊ด ซึ่งถือว่าเป็นหัวใจสำคัญในการพัฒนา สร้างสรรค์ให้เกิดชุดโปรเเกรม หรือซอฟต์เเวร์ใหม่ ๆ ที่เราใช้กันอยู่ในปัจจุบัน

ในรายงานนี้ทางคณะผู้จัดทำได้รวบรวมเนื้อหา เเละข้อมูลที่น่าสนใจต่อการเขียนโค๊ด (Code Development) บนระบบปฎิบัติการ Linux ซึ่งประกอบไปด้วยเนื้อหาดังต่อไปนี้

-   [Script](https://github.com/misterfocusth/Code-Development-Group-02/tree/main/185%20Script)
-   [Debugger](https://github.com/misterfocusth/Code-Development-Group-02/tree/main/21%20Debugger)
-   [Compiler](https://github.com/misterfocusth/Code-Development-Group-02/tree/main/211%20Compiler)
-   [Interpreter](https://github.com/misterfocusth/Code-Development-Group-02/tree/main/225%20Interpreter)
-   [Development Tools](https://github.com/misterfocusth/Code-Development-Group-02/tree/main/27%20Development%20Tools)
-   [Web Development Tools](https://github.com/misterfocusth/Code-Development-Group-02/tree/main/219%20Web%20Development%20Tools)

รายงานนี้เป็นส่วนหนึ่งของรายวิชาโครงสร้างระบบคอมพิวเตอร์และระบบปฏิบัติการ 06016412 (COMPUTER SYSTEMS ORGANIZATION AND OPERATING SYSTEM) ภาคเรียนที่ 2 ปีการศึกษา 2566 คณะเทคโนโลยีสารสนเทศ สถาบันเทคโนโลยีพระจอมเกล้าเจ้าคุณทหารลาดกระบัง

## Overview (ภายรวม)

1.  **Script** การทำงานในแบบ Command-line interopreter ผ่าน Shell ทำงานได้เปรียบเสมือนภาษา Program ชนิดหนึ่ง Script ช่วยให้ผู้ใช้งานสามารถทำงานได้รวดเร็วมากยิ่งขึ้น โดยการรวมเอาคำสั่งและเงื่อนไขที่ผู้ใช้ต้องการใส่ลงใน File และทำการ Execute File
2.  **Debugger เ**ครื่องมือ Software ที่ Developer ใช้เพื่อระบุและแก้ไขปัญหาในโปรแกรมคอมพิวเตอร์ มีสภาพแวดล้อมที่มีการควบคุมสําหรับการตรวจสอบและวิเคราะห์การดําเนินการของโปรแกรม
3.  **Compiler** กระบวนการแปลงโค้ดภาษาโปรแกรม (Source Code) ไปเป็นภาษาเครื่อง (Machine Code) ที่ CPU เข้าใจและสามารถทำงานได้
4.  **Web Development Tools** เครื่องมือที่ช่วยให้นักพัฒนาเว็บ สามารถที่จะทดสอบ หรือ Debug เว็บไซต์ที่พัฒนาขึ้นมาได้ โดยนักพัฒนาส่วนมากมักจะเลือกพัฒนาตัวเว็บโดยใช้ Website Builders หรือพัฒนาใน Integrated Development Environment (IDE) ซึ่งเป็นเครื่องมือที่ช่วยในการเขียนโค๊ด หรือทดสอบ Source Code เเต่ในการพัฒนาเว็บในบางครั้งนักพัฒนาก็จะต้องมีเครื่องมือเฉพาะสำหรับเว็บ ที่ใช้ในการทดสอบ หรือ Debug ในเเต่ละส่วน หรือเเต่ละ Element บนเว็บ
5.  **Interpreter** โปรแกรมคอมพิวเตอร์ที่ทำงานตามชุดคำสั่งที่เขียนไว้ทันที ซึ่งไม่เหมือนกับคอมไพเลอร์ (compiler) ที่แปลชุดคำสั่งจากภาษาคอมพิวเตอร์ภาษา หนึ่งไปเป็นอีกภาษาหนึ่งก่อนทำงาน
6.  **Development Tools** (IDE หรือ Integrated Development Environment) คือ software ที่รวมเอา software ที่จำเป็นในการเขียนโปรแกรมมาอยู่ในที่เดียวกัน

## Tools (เครื่องมือที่ใช้)

-   GitHub ([https://github.com/](https://github.com/))
-   StackEdit ([https://stackedit.io/](https://stackedit.io/))

## Team Member (สมาชิกกลุ่ม)

|Student ID|Name|Selected Topic|Image|
|--|--|--|--|
|65070021|นายกิตติภณ ทัศนเปรมสิน|Debugger| <img src="https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/IMG_1646.jpg?raw=truee" width="125" height="125" />|
|65070027|นางสาวขวัญเนตร ถี่ถ้วน|Development Tools| <img src="https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/IMG_1645.jpg?raw=truee" width="125" height="125" />|
|65070185|นายภูวิศ นุ่นปาน|Script| <img src="https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/IMG_1647.jpg?raw=true" width="125" height="125" />|
|65070211|นางสาวศรุตา โทรัตน์ |Compiler| <img src="https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/IMG_1644.jpg?raw=true" width="125" height="125" />|
|65070219|นายศิลา ภักดีวงษ์|Web Development Tools| <img src="https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/327034314_6025210707536983_7630483055426139603_n.jpg?raw=true" width="125" height="125" />|
|65070225|นายศุภธัช สุวัฒโน|Interpreter| <img src="https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/358070304_2311422129059060_6572322125817828629_n.jpg?raw=true" width="125" height="125" />|



## Present to (เสนอต่อ)

<img src="https://github.com/misterfocusth/Code-Development-Group-02/blob/main/219%20Web%20Development%20Tools/images/Sumet-768x768.jpg?raw=true" width="200" height="200" />

**ผู้ช่วยศาสตราจารย์ ดร. สุเมธ ประภาวัต**

อาจารย์ประจำคณะเทคโนโลยีสารสนเทศ สถาบันเทคโนโลยีพระจอมเกล้าเจ้าคุณทหารลาดกระบัง

[https://www.it.kmitl.ac.th/th/staff/sumet/](https://www.it.kmitl.ac.th/th/staff/sumet/)

[sumet@it.kmitl.ac.th](mailto:sumet@it.kmitl.ac.th)
