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

## Overview (ภาพรวม)

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

## References  (อ้างอิง)
1.  [https://saixiii.com/what-is-shell-script/](https://saixiii.com/what-is-shell-script/)
2.  [https://ftp.psu.ac.th/pub/howto/bash-howto/Shell%20Script.pdf](https://ftp.psu.ac.th/pub/howto/bash-howto/Shell%20Script.pdf)
3.  [https://en.wikipedia.org/wiki/Chmod#:~:text=In%20Unix%20and%20Unix-like,objects%20(files%20and%20directories)](https://en.wikipedia.org/wiki/Chmod#:~:text=In%20Unix%20and%20Unix-like,objects%20(files%20and%20directories)).
4.  [https://th.linux-console.net/?p=15264](https://th.linux-console.net/?p=15264)
5. [https://iot-kmutnb.github.io/blogs/training/gcc_linux/](https://iot-kmutnb.github.io/blogs/training/gcc_linux/)
6. [https://www.geeksforgeeks.org/gdb-step-by-step-introduction/](https://www.geeksforgeeks.org/gdb-step-by-step-introduction/)   
7. [https://www.scaler.com/topics/linux-debugger/](https://www.scaler.com/topics/linux-debugger/)
8. [https://tips.thaiware.com/2059.html](https://tips.thaiware.com/2059.html)
9. [https://ioflood.com/blog/install-gdb-command-linux/](https://ioflood.com/blog/install-gdb-command-linux/)
10.  [https://gcc.gnu.org/onlinedocs/gcc/](https://gcc.gnu.org/onlinedocs/gcc/):  [https://gcc.gnu.org/onlinedocs/gcc/](https://gcc.gnu.org/onlinedocs/gcc/)
11.  [https://lldb.llvm.org/](https://lldb.llvm.org/):  [https://lldb.llvm.org/](https://lldb.llvm.org/)
12.  [https://gcc.gnu.org/onlinedocs/gcc/](https://gcc.gnu.org/onlinedocs/gcc/):  [https://gcc.gnu.org/onlinedocs/gcc/](https://gcc.gnu.org/onlinedocs/gcc/):  [https://gcc.gnu.org/onlinedocs/gcc/](https://gcc.gnu.org/onlinedocs/gcc/):  [https://gcc.gnu.org/onlinedocs/gcc/](https://gcc.gnu.org/onlinedocs/gcc/)
13.   [https://www.gnu.org/software/make/manual/make.html](https://www.gnu.org/software/make/manual/make.html):  [https://www.gnu.org/software/make/manual/make.html](https://www.gnu.org/software/make/manual/make.html)
14.  [https://cmake.org/cmake/help/latest/index.html](https://cmake.org/cmake/help/latest/index.html):  [https://cmake.org/cmake/help/latest/index.html](https://cmake.org/cmake/help/latest/index.html)
15.   [https://docs.gradle.org/current/](https://docs.gradle.org/current/):  [https://docs.gradle.org/current/](https://docs.gradle.org/current/)
16.  [https://docs.npmjs.com/](https://docs.npmjs.com/):  [https://docs.npmjs.com/](https://docs.npmjs.com/)
17.   [https://dnf.readthedocs.io/en/latest/](https://dnf.readthedocs.io/en/latest/):  [https://dnf.readthedocs.io/en/latest/](https://dnf.readthedocs.io/en/latest/)
18.   [https://docs.docker.com/](https://docs.docker.com/):  [https://docs.docker.com/](https://docs.docker.com/)
19.   [https://docs.ansible.com/](https://docs.ansible.com/):  [https://docs.ansible.com/](https://docs.ansible.com/)
20.   [https://clang.llvm.org/](https://clang.llvm.org/):  [https://clang.llvm.org/](https://clang.llvm.org/):  [https://clang.llvm.org/](https://clang.llvm.org/):  [https://clang.llvm.org/](https://clang.llvm.org/)
21.  [https://doc.rust-lang.org/book/](https://doc.rust-lang.org/book/):  [https://doc.rust-lang.org/book/](https://doc.rust-lang.org/book/):  [https://doc.rust-lang.org/book/](https://doc.rust-lang.org/book/):  [https://doc.rust-lang.org/book/](https://doc.rust-lang.org/book/)
22.   [https://lld.llvm.org/](https://lld.llvm.org/):  [https://lld.llvm.org/](https://lld.llvm.org/):  [https://lld.llvm.org/](https://lld.llvm.org/):  [https://lld.llvm.org/](https://lld.llvm.org/)
23.    [https://www.atlassian.com/continuous-delivery/principles](https://www.atlassian.com/continuous-delivery/principles):  [https://www.atlassian.com/continuous-delivery/principles](https://www.atlassian.com/continuous-delivery/principles):  [https://www.atlassian.com/continuous-delivery/principles](https://www.atlassian.com/continuous-delivery/principles):  [https://www.atlassian.com/continuous-delivery/principles](https://www.atlassian.com/continuous-delivery/principles)
1.  [https://en.wikipedia.org/wiki/Web_development_tools](https://en.wikipedia.org/wiki/Web_development_tools)
2.  [](https://th.wikipedia.org/wiki/%E0%B9%80%E0%B8%AD%E0%B8%9E%E0%B8%B5%E0%B8%97%E0%B8%B5_(%E0%B8%8B%E0%B8%AD%E0%B8%9F%E0%B8%95%E0%B9%8C%E0%B9%81%E0%B8%A7%E0%B8%A3%E0%B9%8C))[https://th.wikipedia.org/wiki/เอพีที_(ซอฟต์แวร์)](https://th.wikipedia.org/wiki/%E0%B9%80%E0%B8%AD%E0%B8%9E%E0%B8%B5%E0%B8%97%E0%B8%B5_(%E0%B8%8B%E0%B8%AD%E0%B8%9F%E0%B8%95%E0%B9%8C%E0%B9%81%E0%B8%A7%E0%B8%A3%E0%B9%8C))
3.  [https://devhub.in.th/blog/what-is-web-server](https://devhub.in.th/blog/what-is-web-server)
4.  [](https://www.itgenius.co.th/article/%E0%B9%80%E0%B8%84%E0%B8%A3%E0%B8%B7%E0%B9%88%E0%B8%AD%E0%B8%87%E0%B8%A1%E0%B8%B7%E0%B8%AD%E0%B8%97%E0%B8%B5%E0%B9%88%E0%B9%83%E0%B8%8A%E0%B9%89%E0%B9%83%E0%B8%99%E0%B8%81%E0%B8%B2%E0%B8%A3%E0%B8%9E%E0%B8%B1%E0%B8%92%E0%B8%99%E0%B8%B2%E0%B9%80%E0%B8%A7%E0%B9%87%E0%B8%9A%E0%B9%84%E0%B8%8B%E0%B8%95%E0%B9%8C.html)[https://www.itgenius.co.th/article/เครื่องมือที่ใช้ในการพัฒนาเว็บไซต์.html](https://www.itgenius.co.th/article/%E0%B9%80%E0%B8%84%E0%B8%A3%E0%B8%B7%E0%B9%88%E0%B8%AD%E0%B8%87%E0%B8%A1%E0%B8%B7%E0%B8%AD%E0%B8%97%E0%B8%B5%E0%B9%88%E0%B9%83%E0%B8%8A%E0%B9%89%E0%B9%83%E0%B8%99%E0%B8%81%E0%B8%B2%E0%B8%A3%E0%B8%9E%E0%B8%B1%E0%B8%92%E0%B8%99%E0%B8%B2%E0%B9%80%E0%B8%A7%E0%B9%87%E0%B8%9A%E0%B9%84%E0%B8%8B%E0%B8%95%E0%B9%8C.html)
5.  [https://www.linuxcapable.com/install-google-chrome-on-ubuntu-linux/](https://www.linuxcapable.com/install-google-chrome-on-ubuntu-linux/)
6.  [https://thaibusinesssearch.com/marketing/web-browser/](https://thaibusinesssearch.com/marketing/web-browser/)
7.  [https://vitux.com/ubuntu-xampp/](https://vitux.com/ubuntu-xampp/)
8.  [https://en.wikipedia.org/wiki/HTML](https://en.wikipedia.org/wiki/HTML)
9.  [http://www.krukikz.com/index.php?option=com_content&view=article&id=119&Itemid=152](http://www.krukikz.com/index.php?option=com_content&view=article&id=119&Itemid=152)
10.  [https://en.wikipedia.org/wiki/CSS](https://en.wikipedia.org/wiki/CSS)
11.  [https://www.w3schools.com/js/](https://www.w3schools.com/js/)
12.  [https://dev.to/varunprashar5/how-javascript-engine-s-work-3cb0](https://dev.to/varunprashar5/how-javascript-engine-s-work-3cb0)
13.  [https://aws.amazon.com/th/what-is/ide/](https://aws.amazon.com/th/what-is/ide/)
