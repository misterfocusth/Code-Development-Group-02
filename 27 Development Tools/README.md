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
   
        # yum update -y
    

3. ใช้คำสั่งนี้เพื่อดู package groups ที่สามารถติดตั้งได้

        # yum group list
        #yum groupinstall “GNOME Desktop” “Graphical Administration Tools” -y

![](https://blog.readyidc.com/wp-content/uploads/2019/02/terminal-1.png)

ที่มา: https://blog.readyidc.com/wp-content/uploads/2019/02/terminal-1.png

3. โดยเราจะเลือก 3 package group Server with GUI, GNOME Desktop และ Graphical Administration Tools เพื่อลง GNOME โดยเราใช้คำสั่งด้านล่างนี้เพื่อติดตั้ง

        #yum groupinstall “GNOME Desktop” “Graphical Administration Tools” -y

![](https://blog.readyidc.com/wp-content/uploads/2019/02/terminal-2.png)

ที่มา: https://blog.readyidc.com/wp-content/uploads/2019/02/terminal-2.png

4. ใช้คำสั่ง นี้เพื่อเปิดหน้า GUI 

![](https://blog.readyidc.com/wp-content/uploads/2019/02/terminal-6.png)

    #startx

ที่มา:  https://blog.readyidc.com/wp-content/uploads/2019/02/terminal-6.png


**Optional :** ถ้าเราอยากให้ตัว GNOME เปิดทันที หลังจาก reboot โดยไม่ต้องใช้คำสั่งด้านบน

	#ln -sf /lib/systemd/system/runlevel5.target /etc/systemd/system/default.target

![](https://blog.readyidc.com/wp-content/uploads/2019/02/terminal-4.png)

ที่มา: https://blog.readyidc.com/wp-content/uploads/2019/02/terminal-4.png
  

5. หลังจากเปิด GNOME GUI ให้ทำการ Configure ของ ภาษา, เวลา, username และ password เท่านี้ก็เป็นอันเสร็จสิ้น พร้อมใช้งาน GNOME Desktop GUI

![](https://blog.readyidc.com/wp-content/uploads/2019/02/desktop-1.png)

ที่มา: https://blog.readyidc.com/wp-content/uploads/2019/02/desktop-1.png

![](https://blog.readyidc.com/wp-content/uploads/2019/02/desktop2-1.png)

ที่มา: https://blog.readyidc.com/wp-content/uploads/2019/02/desktop2-1.png

![](https://blog.readyidc.com/wp-content/uploads/2019/02/desktop3.5-1.png)

ที่มา: https://blog.readyidc.com/wp-content/uploads/2019/02/desktop3.5-1.png

![](https://blog.readyidc.com/wp-content/uploads/2019/02/desktop3.6-1.png)

ที่มา: https://blog.readyidc.com/wp-content/uploads/2019/02/desktop3.6-1.png

![](https://blog.readyidc.com/wp-content/uploads/2019/02/desktop3.7-1.png)

ที่มา: https://blog.readyidc.com/wp-content/uploads/2019/02/desktop3.7-1.png

![](https://blog.readyidc.com/wp-content/uploads/2019/02/desktop3-1.png)

ที่มา: https://blog.readyidc.com/wp-content/uploads/2019/02/desktop3-1.png

![](https://blog.readyidc.com/wp-content/uploads/2019/02/desktop4-1.png)

ที่มา: https://blog.readyidc.com/wp-content/uploads/2019/02/desktop4-1.png

## Eclipse คืออะไร ?

Eclipse คือโปรแกรมที่ใช้สำหรับพัฒนาภาษาได้หลายภาษา โปรแกรม Eclipse เป็นโปรแกรมหนึ่งที่ใช้ในการพัฒนา Application Server ได้อย่างมีประสิทธิภาพ และเป็นซอฟต์แวร์ Open Source ที่พัฒนาขึ้นเพื่อใช้โดยนักพัฒนาเอง ทำให้ความก้าวหน้าในการพัฒนาของ Eclipse เป็นไปอย่างต่อเนื่องและรวดเร็ว

Eclipse คือโปรแกรมที่ใช้สำหรับพัฒนาภาษาได้หลายภาษา ซึ่งโปรแกรม Eclipse เป็นโปรแกรมหนึ่งที่ใช้ในการพัฒนา Application Server ได้อย่างมีประสิทธิภาพ และเนื่องจาก Eclipse เป็นซอฟต์แวร์ Open Source ที่พัฒนาขึ้นเพื่อใช้โดยนักพัฒนาเอง ทำให้ความก้าวหน้าในการพัฒนาของ Eclipse เป็นไปอย่างต่อเนื่องและรวดเร็ว

Eclipse มีองค์ประกอบหลักที่เรียกว่า Eclipse Platform ซึ่งให้บริการพื้นฐานหลักสำหรับรวบรวมเครื่องมือต่างๆจากภายนอกให้สามารถเข้ามาทำงานร่วมกันในสภาพแวดล้อมเดียวกัน และมีองค์ประกอบที่เรียกว่า Plug-in Development Environment (PDE) ซึ่งใช้ในการเพิ่มความสามารถในการพัฒนาซอฟต์แวร์มากขึ้น เครื่องมือภายนอกจะถูกพัฒนาในรูปแบบที่เรียกว่า Eclipse plug-ins ดังนั้นหากต้องการให้ Eclipse ทำงานใดเพิ่มเติม ก็เพียงแต่พัฒนา plugin สำหรับงานนั้นขึ้นมา และนำ Plug-in นั้นมาติดตั้งเพิ่มเติมให้กับ Eclipse ที่มีอยู่เท่านั้น Eclipse Plug-in ที่มีมาพร้อมกับ Eclipse เมื่อเรา download มาครั้งแรกก็คือองค์ประกอบที่เรียกว่า Java Development Toolkit (JDT) ซึ่งเป็นเครื่องมือในการเขียนและ Debug โปรแกรมภาษา Java

ข้อดีของโปรแกรม Eclipse คือ ติดตั้งง่าย สามารถใช้ได้กับ J2SDK ได้ทุกเวอร์ชั่น รองรับภาษาต่างประเทศอีกหลายภาษา มี plugin ที่ใช้เสริมประสิทธิภาพของโปรแกรม สามารถทำงานได้กับไฟล์หลายชนิด เช่น HTML, Java, C, JSP, EJB, XML และ GIF และที่สำคัญเป็นฟรีเเวร์ ใช้งานได้กับระบบปฏิบัติการ Windows, Linux และ Mac OS

## ขั้นตอนการติดตั้ง Eclipse บน Ubuntu

Eclipse เป็น IDE ที่นิยมมากในปัจจุบัน วันนี้จะมานำเสนอวิธีติดตั้ง Eclipse สำหรับคนที่ใช้ Ubuntu ขั้นตอนการติดตั้ง Eclipse บน Ubuntu สามารถติดตั้งได้ 3 วิธี ดังนี้

### ติดตั้งผ่าน Ubuntu Software Center

![ติดตั้งผ่าน Ubuntu Software Center](https://raw.githubusercontent.com/Devahoy/devahoy-assets/master/images/2014/03/ubuntu-software-center.png)

ที่มา: https://raw.githubusercontent.com/Devahoy/devahoy-assets/master/images/2014/03/ubuntu-software-center.png

ขั้นตอนการติดตั้งก็เพียงแค่เปิด Ubuntu Software Center จากนั้น Search หาคำว่า 'Eclipse' วิธีการนี้ น่าจะเป็นวิธีการที่สะดวกที่สุด แต่ข้อเสียคือ จะไม่ใช่เวอร์ชั่นล่าสุด โดยเวอร์ชั่นที่สูงสุดใน Ubuntu Software Center คือ 3.8 แต่ปัจจุบัน Eclipse ออกเวอร์ชั่น Kepler 4.3 แล้ว

### ติดตั้งผ่าน Command-Line

ติดตั้งผ่าน Ubuntu Software Center เพียงแต่ไม่มีหน้าตา UI มาให้ แค่ใช้คำสั่งผ่าน command line แทน วิธีการติดตั้งคือ

    sudo apt-get install eclipse


![ผ่าน command-line](https://raw.githubusercontent.com/Devahoy/devahoy-assets/master/images/2014/03/terminal.png)

ที่มา:  https://raw.githubusercontent.com/Devahoy/devahoy-assets/master/images/2014/03/terminal.png

## โหลดจากเว็บ Eclipse.org

 1. เข้าเว็บไซต์ [Eclipse](http://www.eclipse.org/downloads/)
 
![ดาวน์โหลด Eclipse](https://raw.githubusercontent.com/Devahoy/devahoy-assets/master/images/2014/03/eclipse-download.jpg)

ที่มา: https://raw.githubusercontent.com/Devahoy/devahoy-assets/master/images/2014/03/eclipse-download.jpg

เลือก  **Eclipse Standard 4.3.2, 199 MB**  หากใครต้องการที่จะเขียนพวก Java EE ด้วย ก็เลือก  **Eclipse IDE for Java EE Developers, 248 MB**

ทำการเลือก OS ที่ต้องการ จากนั้นทำการดาวน์โหลด หลังจากดาวน์โหลดเสร็จสิ้น จะได้ไฟล์  

> eclipse-standard-kepler-SR2-linux-gtk-x86_64.tar.gz

ไปที่โฟลเดอร์ที่ดาวน์โหลดมา ถ้าไม่ได้เลือกอะไร จะอยู่ที่ /Downloads ทำการ Extract ออกมา โดยใช้คำสั่ง

    cd /home/ชื่อยูเซอร์/Downloads tar -zxvf eclipse-standard-kepler-SR2-linux-gtk-x86_64.tar.gz

เมื่อถึงขั้นตอนนี้ จะได้โฟลเดอร์ eclipse มาแล้ว ทำการย้ายไปไว้ที่ /opt (โฟลเดอร์ใหม่ ใน File System /opt หรือจะโฟลเดอร์ใน /home/ ก็แล้วแต่ชอบ) 

    sudo mv eclipse /opt/

ทำการเพิ่ม Permission ให้กับโฟลเดอร์ eclipse

    cd /opt/ sudo chown -R root:root eclipse sudo chmod -R +r eclipse

ทำให้ eclipse สามารถรันได้ โดยเปลี่ยนpermission และแก้ไข path ที่อยู่ของ eclipse

    sudo touch /usr/bin/eclipse sudo chmod 755 /usr/bin/eclipse

จากนั้นทำการเปิดไฟล์ eclipse ใน  `/usr/bin`  ด้วย gedit หรือ nano

    sudo gedit /usr/bin/eclipse

เพิ่มด้านล่างนี้ลงไป และกดเซฟ

    #!/bin/sh export ECLIPSE_HOME="/opt/eclipse"
    ECLIPSE_HOME/eclipse *

ทำการเพิ่ม icon ให้โชว์ที่หน้า Dash Home

## ทำความเข้าใจกับ Library ที่ใช้ร่วมกันใน Linux

### Linux Basics: Static Libraries vs. Dynamic Libraries

Dynamic Libraries

## References

 - https://www.aosoft.co.th/article/312/Eclipse-%E0%B8%84%E0%B8%B7%E0%B8%AD%E0%B8%AD%E0%B8%B0%E0%B9%84%E0%B8%A3.html
 - https://th.linux-console.net/?p=666
 - https://www.eclipse.org/
 - https://askubuntu.com/questions/80013/how-to-pin-eclipse-to-the-unity-launcher
 - https://askubuntu.com/questions/26632/how-to-install-eclipse
 - https://www.ert.co.th/ide/#IDE-2


