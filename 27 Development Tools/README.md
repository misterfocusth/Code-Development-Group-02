# Development Tools

## Content

 - [IDE](https://github.com/misterfocusth/Code-Development-Group-02/tree/main/27%20Development%20Tools#ide-%E0%B8%84%E0%B8%B7%E0%B8%AD%E0%B8%AD%E0%B8%B0%E0%B9%84%E0%B8%A3)
 - [Eclipse](https://github.com/misterfocusth/Code-Development-Group-02/tree/main/27%20Development%20Tools#eclipse-%E0%B8%84%E0%B8%B7%E0%B8%AD%E0%B8%AD%E0%B8%B0%E0%B9%84%E0%B8%A3-)
 - [Library](https://github.com/misterfocusth/Code-Development-Group-02/tree/main/27%20Development%20Tools#%E0%B8%97%E0%B8%B3%E0%B8%84%E0%B8%A7%E0%B8%B2%E0%B8%A1%E0%B9%80%E0%B8%82%E0%B9%89%E0%B8%B2%E0%B9%83%E0%B8%88%E0%B8%81%E0%B8%B1%E0%B8%9Alibrary%E0%B8%97%E0%B8%B5%E0%B9%88%E0%B9%83%E0%B8%8A%E0%B9%89%E0%B8%A3%E0%B9%88%E0%B8%A7%E0%B8%A1%E0%B8%81%E0%B8%B1%E0%B8%99%E0%B9%83%E0%B8%99-linux)

## IDE คืออะไร

IDE หรือ Integrated Development Environment คือ software ที่รวมเอา software ที่จำเป็นในการเขียนโปรแกรมมาอยู่ในที่เดียวกัน นั่นคือ โดยปกติแล้วเวลาที่เราจะเขียนโปแกรมอะไรสักอย่างนั้น เราต้องใช้ software หลายตัวร่วมด้วยช่วยกัน เช่น

1.  text editor คือ software ที่เราใช้เขียน code โดยใช้ software อะไรก็ได้ ที่เขียนตัวหนังสือลงไปได้
2.  compiler คือ software ที่ทำหน้าที่ แปลภาษาที่เราเขียน ซึ่งอาจเป็นภาษา c/c++ หรือภาษาอื่น ๆ ให้เป็นภาษาเครื่อง ที่ computer หรือ microcontroller เข้าใจ ซึ่ง compiler ก็มีหลายตัว ขึ้นอยู่กับว่าเราจะเขียนภาษาอะไร และ โปรแกรมที่เราเขียนนั้นจะไปใช้บนอะไร หรือ microcontroller ตัวไหน
3.  linker คือ software ที่ทำหน้าที่เชื่อม code ที่ compile แล้วเข้าด้วยกันในกรณีที่เราใช้ library
4.  uploader หรือ programmer คือ software ที่ทำหน้าที่ upload code ที่ compile และ link เสร็จเรียบร้อยแล้ว ใส่เข้าไปใน microcontroller
5.  debugger คือ software ที่ทำหน้าที่ช่วยให้เราเห็น register หรือ memory หรือ สถานการณ์ทำงานของโปรแกรมที่เราเขียนว่าทำงานอย่างไร ช่วยให้เราหาจุดบกพร่องและแก้ปัญหาได้ง่ายขึ้น

ในบางระบบ อาจมีมากกว่าหรือน้อยกว่านี้บ้าง จะเห็นว่ากว่าจะเขียนโปรแกรมจนใช้งานได้นั้นมีขั้นตอน และ software ที่เกี่ยวข้องหลายตัว ดังนั้นเพื่อความสะดวกจึงได้มีการสร้าง software เพื่อรวมการเรียกใช้ software เหล่านี้เข้าด้วยกัน ซึ่งก็คือ IDE หรือ Integrated Development Environment นั่นเอง

## คุณสมบัติหลักที่สำคัญของ IDE

### 1. Code Editor

Code Editor หรือโปรแกรมที่ใช้สำหรับการเขียน แก้ไข และการจัดระเบียบโค้ด โดยตัว Code Editor จะมีคุณสมบัติหลักๆคือ  Syntax Highlighting ที่สามารถจัดรูปแบบโค้ดไม่ว่าจะเป็นความหนาบางของตัวอักษร การใช้สีเพื่อให้แยกส่วนของโค้ดได้ชัดเจนยิ่งขึ้น, Code Completion ช่วยในการเติมโค้ดหรือแนะนำคำสั่งโค้ดที่เรากำลังจะพิมพ์มาให้เลือกและ Code Snippets ที่สร้างชุดโค้ดสำเร็จรูปหรือโค้ดที่มีรูปแบบเดิมๆเพื่อให้สามารถเขียนโค้ดได้สะดวก รวดเร็วยิ่งขึ้น

### 2. Build and Compilation Tools

IDE มีเครื่องมือสำหรับการ  Compiler และ Interpreter โค้ดที่เขียนด้วยภาษาโปรแกรมต่างๆ โดยจะทำการแปลงภาษาที่ผู้เขียนโปรแกรมเขียนขึ้นมาไปเป็นภาษาเครื่อง (Machine Language) ที่คอมพิวเตอร์เข้าใจได้แทน รวมถึงสามารถ Compiler โค้ดได้อัตโนมัติและตรวจหาข้อผิดพลาดที่ซ่อนอยู่ได้ทำให้นักพัฒนาตรวจจับและแก้ไขปัญหาได้อย่างรวดเร็ว

### 3. Debugging Capabilities

Debuggers เป็นเครื่องมือสำหรับการแก้ไขข้อผิดพลาดหรือจุดบกพร่อง  (Debugging) ที่พบจากการทดสอบโค้ด  ฟังก์ชัน  Debugging ช่วยให้นักพัฒนาสามารถตั้ง  Breakpoints ตรวจสอบตัวแปร และติดตามการทำงานของโปรแกรมได้ ดังนั้นนักพัฒนาจึงมั่นใจได้ว่าโค้ดของพวกเขาจะสามารถทำงานได้ตามที่คาดหวังไว้.

### 4. Version Control Integration

 IDE รวมตัวเข้ากับระบบ Version Control อย่าง [Git](https://www.ert.co.th/git-%e0%b9%81%e0%b8%a5%e0%b8%b0-github-%e0%b8%95%e0%b9%88%e0%b8%b2%e0%b8%87%e0%b8%81%e0%b8%b1%e0%b8%99%e0%b8%ad%e0%b8%a2%e0%b9%88%e0%b8%b2%e0%b8%87%e0%b9%84%e0%b8%a3/) ที่ทำให้นักพัฒนาจัดการ Codebase ได้อย่างมีประสิทธิภาพมากขึ้น ซึ่ง Version Control นอกจากจะช่วยให้นักพัฒนาติดตามการเปลี่ยนแปลงร่วมกันกับเพื่อนร่วมทีม ยังช่วยให้นักพัฒนาสามารถย้อนไฟล์บางไฟล์ก่อนหน้าได้หากเกิดข้อผิดพลาดขึ้น

### 5. Extensibility and Customization

IDE นำเสนอการทำงานผ่าน Plugins และ Extension ที่ช่วยพัฒนาประสิทธิภาพการทำงานของตัวมันเองรวมถึงรองรับภาษาโปรแกรม เฟรมเวิร์ก และเครื่องมือพิเศษอีกด้วย นอกจากนี้นักพัฒนายังสามารถปรับแต่ง IDE ของตัวเองได้โดยอาจจะเลือกชุดสีหรือแบบที่แตกต่างกันออกไปตามความชอบและ Workflow ที่เหมาะสม


## IDE ยอดนิยม

### 1. Visual Studio
![Tricks and tips for VSCode Beginners | by Komal Khetlani | Dev Genius](https://miro.medium.com/v2/resize:fit:480/0*q_2SlZs2OUPK0Ujv.png)

ที่มา: https://miro.medium.com/v2/resize:fit:480/0*q_2SlZs2OUPK0Ujv.png

Visual Studio ประกอบไปด้วยคุณสมบัติและเครื่องมือที่หลากหลายในการสร้างหรือพัฒนาโปรแกรมสำเร็จรูปอย่างเว็บไซต์และแอปพลิเคชัน โดยระบบที่รองรับการทำงานนั้นมี Window, Pocket PC, Smartphoneและ  Web browser


### 2. IntelliJ IDEA
![What is Intellij IDEA - A Comprehensive Guide](https://www.simplilearn.com/ice9/free_resources_article_thumb/Intellij_IDEA.jpg)

ที่มา: https://www.simplilearn.com/ice9/free_resources_article_thumb/Intellij_IDEA.jpg

IDE เน้นการพัฒนา Java เป็นหลัก แต่ยังสามารถรองรับภาษาอื่นๆได้เช่น Kotlin, Scala, Dart, PHP ฟีเจอร์หลักๆของ IntelliJ IDEA ได้แก่ Code Completion และ Code Inspection เป็นต้น


### 3. PyCharm
![PyCharm's top features. [Hidden] qualities of one of the most… | by Nicolò  Gasparini | Analytics Vidhya | Medium](https://miro.medium.com/v2/resize:fit:2000/1*gYFLCqNfVX3qvwnoNwFFNA.png)

ที่มา: https://miro.medium.com/v2/resize:fit:2000/1*gYFLCqNfVX3qvwnoNwFFNA.png

IDE พิเศษสำหรับ Python ตั้งแต่การวิเคราะห์โค้ด การดีบัก และการทดสอบเฟรมเวิร์ก ด้วยความช่วยเหลืออันชาญฉลาดของ PyCharm ทำให้นักพัฒนาสามารถเพิ่มประสิทธิภาพการเขียนโค้ดของ Python ได้อย่างมาก

## ตัวอย่างการติดตั้ง Desktop Environment “GNOME” ลงใน CentOS 7

1. ก่อนที่เราจะติดตั้ง ให้ทำการ update ก่อน โดยใช้คำสั่ง

   #yum update -y

3. ใช้คำสั่งนี้เพื่อดู package groups ที่สามารถติดตั้งได้

        # yum group list

![](https://blog.readyidc.com/wp-content/uploads/2019/02/terminal-1.png)

ที่มา: https://blog.readyidc.com/wp-content/uploads/2019/02/terminal-1.png

3. โดยเราจะเลือก 3 package group Server with GUI, GNOME Desktop และ Graphical Administration Tools เพื่อลง GNOME โดยเราใช้คำสั่งด้านล่างนี้เพื่อติดตั้ง

    _#yum groupinstall “GNOME Desktop” “Graphical Administration Tools” -y_

![](https://blog.readyidc.com/wp-content/uploads/2019/02/terminal-2.png)
ที่มา: https://blog.readyidc.com/wp-content/uploads/2019/02/terminal-2.png

4. ใช้คำสั่ง นี้เพื่อเปิดหน้า GUI

_#startx_

![](https://blog.readyidc.com/wp-content/uploads/2019/02/terminal-6.png)

  

**Optional :** ถ้าเราอยากให้ตัว GNOME เปิดทันที หลังจาก reboot โดยไม่ต้องใช้คำสั่งด้านบน

_#ln -sf /lib/systemd/system/runlevel5.target /etc/systemd/system/default.target_

![](https://blog.readyidc.com/wp-content/uploads/2019/02/terminal-4.png)

  

5.หลังจากเปิด GNOME GUI ให้ทำการ Configure ของ ภาษา, เวลา, username และ password เท่านี้ก็เป็นอันเสร็จสิ้น พร้อมใช้งาน GNOME Desktop GUI

  

![](https://blog.readyidc.com/wp-content/uploads/2019/02/desktop-1.png)

![](https://blog.readyidc.com/wp-content/uploads/2019/02/desktop2-1.png)

![](https://blog.readyidc.com/wp-content/uploads/2019/02/desktop3.5-1.png)

![](https://blog.readyidc.com/wp-content/uploads/2019/02/desktop3.6-1.png)

![](https://blog.readyidc.com/wp-content/uploads/2019/02/desktop3.7-1.png)

![](https://blog.readyidc.com/wp-content/uploads/2019/02/desktop3-1.png)

![](https://blog.readyidc.com/wp-content/uploads/2019/02/desktop4-1.png)

## Eclipse คืออะไร ?

Eclipse คือโปรแกรมที่ใช้สำหรับพัฒนาภาษาได้หลายภาษา โปรแกรม Eclipse เป็นโปรแกรมหนึ่งที่ใช้ในการพัฒนา Application Server ได้อย่างมีประสิทธิภาพ และเป็นซอฟต์แวร์ Open Source ที่พัฒนาขึ้นเพื่อใช้โดยนักพัฒนาเอง ทำให้ความก้าวหน้าในการพัฒนาของ Eclipse เป็นไปอย่างต่อเนื่องและรวดเร็ว

Eclipse คือโปรแกรมที่ใช้สำหรับพัฒนาภาษาได้หลายภาษา ซึ่งโปรแกรม Eclipse เป็นโปรแกรมหนึ่งที่ใช้ในการพัฒนา Application Server ได้อย่างมีประสิทธิภาพ และเนื่องจาก Eclipse เป็นซอฟต์แวร์ Open Source ที่พัฒนาขึ้นเพื่อใช้โดยนักพัฒนาเอง ทำให้ความก้าวหน้าในการพัฒนาของ Eclipse เป็นไปอย่างต่อเนื่องและรวดเร็ว

Eclipse มีองค์ประกอบหลักที่เรียกว่า Eclipse Platform ซึ่งให้บริการพื้นฐานหลักสำหรับรวบรวมเครื่องมือต่างๆจากภายนอกให้สามารถเข้ามาทำงานร่วมกันในสภาพแวดล้อมเดียวกัน และมีองค์ประกอบที่เรียกว่า Plug-in Development Environment (PDE) ซึ่งใช้ในการเพิ่มความสามารถในการพัฒนาซอฟต์แวร์มากขึ้น เครื่องมือภายนอกจะถูกพัฒนาในรูปแบบที่เรียกว่า Eclipse plug-ins ดังนั้นหากต้องการให้ Eclipse ทำงานใดเพิ่มเติม ก็เพียงแต่พัฒนา plugin สำหรับงานนั้นขึ้นมา และนำ Plug-in นั้นมาติดตั้งเพิ่มเติมให้กับ Eclipse ที่มีอยู่เท่านั้น Eclipse Plug-in ที่มีมาพร้อมกับ Eclipse เมื่อเรา download มาครั้งแรกก็คือองค์ประกอบที่เรียกว่า Java Development Toolkit (JDT) ซึ่งเป็นเครื่องมือในการเขียนและ Debug โปรแกรมภาษา Java

ข้อดีของโปรแกรม Eclipse คือ ติดตั้งง่าย สามารถใช้ได้กับ J2SDK ได้ทุกเวอร์ชั่น รองรับภาษาต่างประเทศอีกหลายภาษา มี plugin ที่ใช้เสริมประสิทธิภาพของโปรแกรม สามารถทำงานได้กับไฟล์หลายชนิด เช่น HTML, Java, C, JSP, EJB, XML และ GIF และที่สำคัญเป็นฟรีเเวร์ ใช้งานได้กับระบบปฏิบัติการ Windows, Linux และ Mac OS

### 1. ติดตั้ง Eclipse IDE ใน CentOS, RHEL และ Fedora
ต้องใช้เวอร์ชัน Java 9 หรือสูงกว่าเพื่อติดตั้ง Eclipse IDE และวิธีที่ง่ายที่สุดในการติดตั้ง Oracle Java JDK จากที่เก็บเริ่มต้น

    # yum install java-11-openjdk-devel
    # java -version
    
จากนั้น เปิดเบราว์เซอร์ ไปที่หน้าดาวน์โหลดอย่างเป็นทางการของ Eclipse และดาวน์โหลดเวอร์ชันล่าสุดของแพ็คเกจ tar เฉพาะสำหรับ## สถาปัตยกรรมการประมวลผลแบบกระจาย Linux ที่ติดตั้งของคุณ
หรือคุณสามารถดาวน์โหลดไฟล์ตัวติดตั้ง  Eclipse IDE ในระบบของคุณผ่านทางยูทิลิตี้ **wget** โดยออกคำสั่งด้านล่าง

    # wget http://ftp.yz.yamagata-u.ac.jp/pub/eclipse/oomph/epp/2020-06/R/eclipse-inst-linux64.tar.gz
    
หลังจากการดาวน์โหลดเสร็จสิ้น ให้ไปที่ไดเร็กทอรีที่มีการดาวน์โหลดแพ็คเกจไฟล์เก็บถาวร และใช้คำสั่งด้านล่างเพื่อเริ่มการติดตั้ง Eclipse IDE

    # tar -xvf eclipse-inst-linux64.tar.gz 
    # cd eclipse-installer/
    # sudo ./eclipse-inst
    
โปรแกรมติดตั้ง Eclipse แสดงรายการ IDE ที่ผู้ใช้ Eclipse ใช้ได้ คุณสามารถเลือกและคลิกที่แพ็คเกจ IDE ที่คุณต้องการติดตั้ง

![](https://th.linux-console.net/common-images/install-eclipse-ide-in-centos-rhel-fedora/Eclipse-Installer.png)

จากนั้น เลือกโฟลเดอร์ที่คุณต้องการติดตั้ง Eclipse

![](https://th.linux-console.net/common-images/install-eclipse-ide-in-centos-rhel-fedora/Choose-Eclipse-IDE-Installation-Folder.png)

เมื่อการติดตั้งเสร็จสิ้น คุณสามารถเปิดใช้ Eclipse ได้แล้ว

![](https://th.linux-console.net/common-images/install-eclipse-ide-in-centos-rhel-fedora/Launch-Eclipse-IDe.png)

![](https://th.linux-console.net/common-images/install-eclipse-ide-in-centos-rhel-fedora/Eclipse-IDE.png)

### ติดตั้ง Eclipse IDE ผ่าน Snap บน Fedora

Snap คือการจัดการแพ็คเกจซอฟต์แวร์ที่ใช้ในการติดตั้งแพ็คเกจของบุคคลที่สามบน Fedora Linux คุณสามารถใช้  snap เพื่อติดตั้ง Eclipse IDE บน Fedora โดยใช้คำสั่งต่อไปนี้

    $ sudo dnf install snapd
    $ sudo ln -s /var/lib/snapd/snap /snap
    $ snap search eclipse
    $ sudo snap install --classic eclipse
    
คุณได้ติดตั้ง Eclipse IDE เวอร์ชันล่าสุดในระบบที่ใช้ Red Hat Linux เรียบร้อยแล้ว

## ทำความเข้าใจกับLibraryที่ใช้ร่วมกันใน Linux

ในการเขียนโปรแกรม ไลบรารีคือกลุ่มของโค้ดที่คอมไพล์ไว้ล่วงหน้าซึ่งสามารถนำมาใช้ซ้ำได้ในโปรแกรม ไลบรารีทำให้ชีวิตของโปรแกรมเมอร์ง่ายขึ้น โดยมีฟังก์ชัน รูทีน คลาส โครงสร้างข้อมูล และอื่นๆ ที่ใช้ซ้ำได้ (เขียนโดยโปรแกรมเมอร์คนอื่น) ซึ่งสามารถใช้ในโปรแกรมของตนได้

ตัวอย่างเช่น หากคุณกำลังสร้างแอปพลิเคชันที่ต้องดำเนินการทางคณิตศาสตร์ คุณไม่จำเป็นต้องสร้างฟังก์ชันทางคณิตศาสตร์ใหม่สำหรับสิ่งนั้น คุณสามารถใช้ฟังก์ชันที่มีอยู่ในไลบรารีสำหรับภาษาโปรแกรมนั้นๆ ได้

ตัวอย่างของไลบรารีใน Linux ได้แก่  **libc**  (ไลบรารี C มาตรฐาน) หรือ  **Glibc**  (เวอร์ชัน GNU ของไลบรารี C มาตรฐาน),  **libcurl**  (ไฟล์หลายโปรโตคอล โอนไลบรารี),  **libcrypt**  (ไลบรารีที่ใช้สำหรับการเข้ารหัส การแฮช และการเข้ารหัสในภาษา C) และอื่นๆ อีกมากมาย

Linux รองรับไลบรารีสองคลาส ได้แก่:

 1. **ไลบรารีแบบสแตติก**  – เชื่อมโยงกับโปรแกรมแบบสแตติก ณ เวลาคอมไพล์
 2. **ไดนามิกหรือไลบรารีที่ใช้ร่วมกัน**  – จะถูกโหลดเมื่อเปิดโปรแกรมและโหลดลงในหน่วยความจำและการรวมเกิดขึ้นเมื่อรันไทม์
 
 ไลบรารีไดนามิกหรือไลบรารีที่ใช้ร่วมกันสามารถจัดประเภทเพิ่มเติมเป็น:
-   **ไลบรารีที่เชื่อมโยงแบบไดนามิก**  – ที่นี่โปรแกรมเชื่อมโยงกับไลบรารีที่ใช้ร่วมกัน และเคอร์เนลจะโหลดไลบรารี (ในกรณีที่ไม่ได้อยู่ในหน่วยความจำ) เมื่อดำเนินการ
-   **ไลบรารีที่โหลดแบบไดนามิก**  – โปรแกรมควบคุมเต็มรูปแบบโดยการเรียกฟังก์ชันด้วยไลบรารี
#### แบบแผนการตั้งชื่อไลบรารีที่ใช้ร่วมกัน

ไลบรารีที่ใช้ร่วมกันมีการตั้งชื่อในสองวิธี: ชื่อไลบรารี (a.k.a  **soname**) และ \ชื่อไฟล์” (พาธสัมบูรณ์ไปยังไฟล์ที่เก็บรหัสไลบรารี)

ตัวอย่างเช่น  **soname**  สำหรับ  **libc**  คือ  **libc.so.6**  โดยที่  **lib**  เป็นคำนำหน้า  **c**  เป็นชื่อที่สื่อความหมาย ดังนั้นหมายถึงวัตถุที่ใช้ร่วมกัน และ  **6**  คือเวอร์ชัน และชื่อไฟล์คือ:  **/lib64/libc.so.6**  โปรดทราบว่าชื่อจริงเป็นลิงก์สัญลักษณ์ไปยังชื่อไฟล์

#### การค้นหาไลบรารีที่ใช้ร่วมกันใน Linux

ไลบรารีที่ใช้ร่วมกันโหลดโดย  **ld.so**  (หรือ  **ld.so.x**) และ  **ld-linux.so**  (หรือ  **ld- linux.so.x**) โปรแกรม โดยที่  **x**  คือเวอร์ชัน ใน Linux  **/lib/ld-linux.so.x**  จะค้นหาและโหลดไลบรารีที่ใช้ร่วมกันทั้งหมดที่ใช้โดยโปรแกรม

โปรแกรมสามารถเรียกไลบรารีโดยใช้ชื่อไลบรารีหรือชื่อไฟล์ และพาธไลบรารีจะจัดเก็บไดเร็กทอรีซึ่งไลบรารีสามารถพบได้ในระบบไฟล์ ตามค่าเริ่มต้น ไลบรารีจะอยู่ใน  **/usr/local/lib**,  **/usr/local/lib64**,  **/usr/lib**  และ  **/usr/lib64**; ไลบรารีการเริ่มต้นระบบอยู่ใน  **/lib**  และ  **/lib64**  อย่างไรก็ตาม โปรแกรมเมอร์สามารถติดตั้งไลบรารีในตำแหน่งที่กำหนดเองได้

เส้นทางของไลบรารีสามารถกำหนดได้ในไฟล์  **/etc/ld.so.conf**  ซึ่งคุณสามารถแก้ไขได้ด้วยตัวแก้ไขบรรทัดคำสั่ง

    # vi /etc/ld.so.conf
   
   บรรทัดในไฟล์นี้สั่งให้เคอร์เนลโหลดไฟล์ใน  **/etc/ld.so.conf.d**  ด้วยวิธีนี้ ผู้ดูแลแพ็คเกจหรือโปรแกรมเมอร์สามารถเพิ่มไดเร็กทอรีไลบรารีที่กำหนดเองลงในรายการค้นหา

หากคุณดูในไดเร็กทอรี  **/etc/ld.so.conf.d**  คุณจะเห็นไฟล์  **.conf**  สำหรับแพ็คเกจทั่วไป (เคอร์เนล, mysql และ postgresql ใน กรณีนี้):

    # ls /etc/ld.so.conf.d
    kernel-2.6.32-358.18.1.el6.x86_64.conf  
    kernel-2.6.32-696.1.1.el6.x86_64.conf  
    mariadb-x86_64.conf
    kernel-2.6.32-642.6.2.el6.x86_64.conf   
    kernel-2.6.32-696.6.3.el6.x86_64.conf  
    postgresql-pgdg-libs.conf
  
 หากคุณดูที่ mariadb-x86_64.conf คุณจะเห็นเส้นทางที่แน่นอนไปยังไลบรารีแพ็คเกจ

    # cat mariadb-x86_64.conf
    /usr/lib64/mysql
  
  วิธีการข้างต้นกำหนดเส้นทางห้องสมุดอย่างถาวร หากต้องการตั้งค่าชั่วคราว ให้ใช้ตัวแปรสภาพแวดล้อม **LD_LIBRARY_PATH** ในบรรทัดคำสั่ง หากคุณต้องการให้การเปลี่ยนแปลงเป็นแบบถาวร ให้เพิ่มบรรทัดนี้ในไฟล์เริ่มต้นเชลล์ **/etc/profile** (ส่วนกลาง) หรือ **~/.profile** (เฉพาะผู้ใช้

    # export LD_LIBRARY_PATH=/path/to/library/file
    
#### การจัดการไลบรารีที่ใช้ร่วมกันใน Linux

ให้เราดูวิธีจัดการกับไลบรารีที่ใช้ร่วมกัน หากต้องการดูรายการการขึ้นต่อกันของไลบรารีที่ใช้ร่วมกันทั้งหมดสำหรับไฟล์ไบนารี คุณสามารถใช้  **ยูทิลิตี ldd**  ผลลัพธ์ของ  **ldd**  จะอยู่ในรูปแบบ:

> library name =>  filename (some hexadecimal value) OR filename (some
> hexadecimal value)  #this is shown when library name can’t be read

คำสั่งนี้แสดงการขึ้นต่อกันของไลบรารีที่ใช้ร่วมกันทั้งหมดสำหรับคำสั่ง ls

    # ldd /usr/bin/ls
หรือ

    # ldd /bin/ls

##### ตัวอย่างผลลัพธ์
    linux-vdso.so.1 =>  (0x00007ffebf9c2000)
	libselinux.so.1 => /lib64/libselinux.so.1 (0x0000003b71e00000)
	librt.so.1 => /lib64/librt.so.1 (0x0000003b71600000)
	libcap.so.2 => /lib64/libcap.so.2 (0x0000003b76a00000)
	libacl.so.1 => /lib64/libacl.so.1 (0x0000003b75e00000)
	libc.so.6 => /lib64/libc.so.6 (0x0000003b70600000)
	libdl.so.2 => /lib64/libdl.so.2 (0x0000003b70a00000)
	/lib64/ld-linux-x86-64.so.2 (0x0000561abfc09000)
	libpthread.so.0 => /lib64/libpthread.so.0 (0x0000003b70e00000)
	libattr.so.1 => /lib64/libattr.so.1 (0x0000003b75600000)

เนื่องจากไลบรารีที่ใช้ร่วมกันสามารถมีอยู่ในไดเร็กทอรีต่างๆ มากมาย การค้นหาผ่านไดเร็กทอรีเหล่านี้ทั้งหมดเมื่อเปิดโปรแกรมจะไม่มีประสิทธิภาพอย่างมาก ซึ่งเป็นข้อเสียอย่างหนึ่งของไดนามิกไลบรารี ดังนั้นจึงมีการใช้กลไกการแคช ซึ่งดำเนินการโดยโปรแกรม  **ldconfig**

ตามค่าเริ่มต้น  **ldconfig**  จะอ่านเนื้อหาของ  **/etc/ld.so.conf**  สร้างลิงก์สัญลักษณ์ที่เหมาะสมในไดเรกทอรีลิงก์แบบไดนามิก จากนั้นเขียนแคชไปยัง  **/etc/ld.so.cache**  ซึ่งจะนำไปใช้โดยโปรแกรมอื่นได้อย่างง่ายดาย

สิ่งนี้สำคัญมากโดยเฉพาะเมื่อคุณเพิ่งติดตั้งไลบรารีที่ใช้ร่วมกันใหม่ หรือสร้างไลบรารีของคุณเอง หรือสร้างไดเร็กทอรีไลบรารีใหม่ คุณต้องเรียกใช้คำสั่ง  **ldconfig**  เพื่อให้การเปลี่ยนแปลงมีผล

    # ldconfig

 หรือ
 

    # ldconfig -v 	#shows files and directories it works with

หลังจากสร้างไลบรารีที่ใช้ร่วมกัน คุณต้องติดตั้ง คุณสามารถย้ายไปยังไดเร็กทอรีมาตรฐานใดก็ได้ที่กล่าวถึงข้างต้นและเรียกใช้คำสั่ง  **ldconfig**

หรือเรียกใช้คำสั่งต่อไปนี้เพื่อสร้างลิงก์สัญลักษณ์จาก  **soname**  ไปยังชื่อไฟล์:

    # ldconfig -n /path/to/your/shared/libraries
หากต้องการเริ่มต้นสร้างไลบรารีของคุณเอง โปรดดูคู่มือนี้จาก [The Linux Documentation Project (TLDP)](https://tldp.org/HOWTO/Program-Library-HOWTO/introduction.html)


## References

 - https://www.mindphp.com/%E0%B8%84%E0%B8%B9%E0%B9%88%E0%B8%A1%E0%B8%B7%E0%B8%AD/73-%E0%B8%84%E0%B8%B7%E0%B8%AD%E0%B8%AD%E0%B8%B0%E0%B9%84%E0%B8%A3/2245-ide-%E0%B8%84%E0%B8%B7%E0%B8%AD%E0%B8%AD%E0%B8%B0%E0%B9%84%E0%B8%A3.html
 - https://aws.amazon.com/th/what-is/ide/
 - https://th.linux-console.net/?p=1836
 - https://www.aosoft.co.th/article/312/Eclipse-%E0%B8%84%E0%B8%B7%E0%B8%AD%E0%B8%AD%E0%B8%B0%E0%B9%84%E0%B8%A3.html
 - https://sumethd.medium.com/%E0%B8%A7%E0%B8%B4%E0%B8%98%E0%B8%B5%E0%B8%81%E0%B8%B2%E0%B8%A3%E0%B8%95%E0%B8%B4%E0%B8%94%E0%B8%95%E0%B8%B1%E0%B9%89%E0%B8%87-gnome-desktop-%E0%B9%80%E0%B8%9E%E0%B8%B7%E0%B9%88%E0%B8%AD-enable-gui-mode-in-rhel-8-5a13e831d0ee
 - https://th.linux-console.net/?p=666
