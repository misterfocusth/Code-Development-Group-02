# Interpreters

ประเภทของ Interpreter และเนื้อหาที่จะกล่าวถึง
1. Shell Interpreter
	* SH
	* Bash
	* Zsh
2. Programming Language Interpreter
 	* Python
	* Perl
	* Ruby
	* Node.js

## Shell Interpreter

Shell Interpreter หรือ **โปรแกรมแปลภาษาเชลล์** เป็นโปรแกรมคอมพิวเตอร์ที่ทำหน้าที่อ่านและดำเนินการคำสั่งที่ผู้ใช้ป้อนเข้ามาผ่านอินเทอร์เฟซบรรทัดคำสั่ง (command line interface) เปรียบเสมือนตัวกลางที่ช่วยให้ผู้ใช้สามารถสื่อสารกับระบบปฏิบัติการและโปรแกรมอื่น ๆ ได้โดยไม่ต้องเขียนโปรแกรม

__หน้าที่หลักของ Interpreter__
-   **อ่านคำสั่ง:**  โปรแกรมแปลภาษาเชลล์จะอ่านคำสั่งที่ผู้ใช้ป้อนเข้ามาผ่านแป้นพิมพ์
-   **แปลคำสั่ง:**  โปรแกรมแปลภาษาเชลล์จะแปลคำสั่งที่อ่านมาเป็นภาษาที่ระบบปฏิบัติการเข้าใจ
-   **ดำเนินการคำสั่ง:**  โปรแกรมแปลภาษาเชลล์จะส่งคำสั่งที่แปลแล้วไปยังระบบปฏิบัติการเพื่อดำเนินการ
-   **แสดงผลลัพธ์:**  โปรแกรมแปลภาษาเชลล์จะแสดงผลลัพธ์ที่ได้จากการดำเนินการของระบบปฏิบัติการ

มี Shell Interpreter หลายประเภทที่ใช้ในระบบปฏิบัติการ Unix-like เช่น Bash, Zsh, Csh, Tcsh แต่ละประเภทมีคุณสมบัติและฟังก์ชันการทำงานที่แตกต่างกัน

### SH

SH หรือที่เรียกกันว่า __Bourne Shell__ เป็น shell หลักสำหรับ Unix โดยที่ถูกเผยแพร่ครั้งแรกในยุค 1970 คิดค้นโดย Stephen Bourne ที่ Bell Labs. SH เป็นที่รู้จักกันถึงในความเรียบง่าย, มีขนาดเล็ก, และเบา

SH ไม่จำเป็นที่จะต้องติดตั้งแยกในภายหลังเนื่องจากเป็น shell หลัก ซึ่งมีติดมากับตอนติดตั้ง Linux อยู่แล้ว

### Bash

Bash หรือที่รู้จักกันด้วยชื่อเต็มว่า Bourne Again SHell เป็น shell รุ่นที่ถูกพัฒนาต่อมาจาก SH โดย Brian Fox สำหรับ GNU Project เพื่อเป็นซอฟต์แวร์ฟรีสำหรับทดแทน Bourne Shell โดยที่ปัจจุบัน Bash เป็น default shell สำหรับหลาย Linux Distributions โดยที่ยังได้มี features จากหลากหลาย shell อื่นเช่น KornShell (ksh) and C shell (csh)

### ข้อแตกต่างระหว่าง SH และ Bash

หลังจากที่เราได้เรียนรู้ถึงที่มาของ SH และ Bash แล้ว เราจะมาทราบถึงข้อแตกต่างระหว่าง SH และ Bash โดยข้อแตกต่างที่น่าสนใจมีดังต่อไปนี้
* ความแตกต่างกันในด้าน Syntax
```bash
# SH Syntax
if  [  $a  -lt  $b  ];  then
echo  "$a is less than $b"
fi
# Bash Syntax
if  [[  $a  -lt  $b  ]];  then
echo  "$a is less than $b"
fi
```
* Bash รองรับค่าตัวแปรแบบ Array
```bash
# Bash Syntax
array=("apple"  "banana"  "cherry")
echo  ${array[1]}  # Outputs "banana"
```
* Bash รองรับ Command Line Editing - กล่าวคือรองรับการย้อนเรียกคำสั่งเก่าๆ ใน history ด้วยปุ่มลูกศร, การใช้ปุ่ม tab สำหรับการทำ command autocomplete, และการลบตัวอักษรที่ได้เขียนไปแล้วด้วยปุ่ม backspace

### Zsh (Z shell)

Zshell หรือที่เรียกกันว่า zsh เป็น Unix shell ที่ถูกพัฒนาต่อมาจาก Bourne shell (SH) โดยที่ได้เอาความสามารถของหลากหลาย shell อื่นๆ มาต่อยอดเช่น Bash, ksh, tcsh

Zsh ถูกพัฒนาโดย Paul Falstad ใน 1990 ระหว่างที่นักศึกษาอยู่ที่ Princeton Univeristy โดยที่ได้รวมความสามารถของ ksh และ tcsh เช่น command-line completion, extended file globbing, การจัดการค่าตัวแปร/array ที่ดีขึ้น, และการคุมสีธีมของตัว prompt

### ข้อแตกต่างระหว่าง Zsh และ Bash

* Zsh รองรับการทำ prompt customization
จากภาพ จะเป็นการปรับแต่งหน้าตาและสีของ prompt ตนเองใน Zsh

	```bash
	PS1="%F{green}%n@%m %F{blue}%~ %f$ "
	```

	![https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/what-is-the-difference-zsh-vs-bash-scripting-in-the-terminal-prompt-customization.jpg](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/what-is-the-difference-zsh-vs-bash-scripting-in-the-terminal-prompt-customization.jpg)

	Zsh รองรับหลากหลายวิธีในการตกแต่ง prompt แต่ว่า Bash จะใช้เครื่องหมาย escape codes ในการบ่งบอกถึงสีและการทำ formatting เพื่อแก้ไข prompt

* Extended Globbing Patterns
 หมายถึงความสามารถในการเลือกกับแก้ไขไฟล์และ directories ผ่านการคัดกรองตามเงื่อนไขต่างๆ โดยใน Zsh script นั้นสามารถใช้งาน pattern เงื่อนไขที่ได้กล่าวไว้ด้วยคำสั่ง **setopt** อย่างเช่นหากต้องการเลือกไฟล์ที่ลงท้ายด้วยนามสกุล .txt ทุกไฟล์ใน directory ปัจจุบัน

	```bash
	setopt extended_glob  
	txt_files=(*.txt)
	```
	แต่ถ้าหากใช้งานใน Bash นั้นจะจำเป็นต้องใช้คำสั่ง **shopt** แทน โดยที่ความแตกต่างระหว่าง Zsh กับ Bash จะเป็น syntax ที่ใช้งาน

### Zsh Installation
ขั้นตอนต่อไปนี้ใช้สำหรับการติดตั้ง Zsh กับ Ubuntu Linux เท่านั้น

#### ขั้นตอนการตรวจสอบว่าติดตั้งและใช้งาน Zsh ถูกต้องหรือไม่
1. รัน `zsh --version` จะแสดงเวอร์ชั่นของ zsh ที่ได้ติดตั้งลงบนเครื่องแล้ว โดยผลลัพธ์ที่คาดหวังคือตั้งแต่เวอร์ชั่น >= 5.0.8
2. รัน `echo $SHELL` บน terminal อันใหม่จะเป็นการแสดงว่ากำลังใช้ shell ตัวใดอยู่ โดยผลลัพธ์ที่คาดหวังคือ `/usr/bin/zsh`

#### ขั้นตอนการติดตั้ง Zsh
1. การติดตั้ง Zsh นั้นมีอยู่ด้วยกัน 2 ทางเลือกได้แก่
	1.1 ติดตั้งด้วยการ compile ตัว [source code](https://zsh.sourceforge.io/Arc/source.html) โดยสามารถดูวิธีได้จาก [Zsh FAQ](https://zsh.sourceforge.io/FAQ/zshfaq01.html#l7)
2. ติดตั้งผ่าน package manager ด้วยการรันคำสั่ง `sudo apt install zsh`
3. หลังจากทำการติดตั้ง Zsh เสร็จสิ้น สามารถเปลี่ยน default shell ได้ด้วยคำสั่ง `chsh -s $(which zsh)` โดยที่ `chsh` เป็นคำสั่งสำหรับการแก้ไข default shell
4. ทำการ logout และ login กลับเข้ามาใหม่และทำการตรวจสอบผลลัพธ์การติดตั้ง

## Programming Languages Interpreter
**Programming Language Interpreter** หรือ **โปรแกรมแปลภาษาแบบทีละบรรทัด** เป็นโปรแกรมคอมพิวเตอร์ที่ทำหน้าที่แปลและรันโค้ดภาษาโปรแกรมแบบทีละบรรทัด ต่างจาก Compiler ที่แปลโค้ดทั้งหมดเป็นภาษาเครื่องก่อนรัน ตัวอย่างภาษาโปรแกรมที่ใช้ Interpreter; Python, JavaScript, Ruby, PHP, Perl, etc

**ข้อดีของ Interpreter:**

-   **พัฒนาโปรแกรมได้รวดเร็ว:**  ไม่จำเป็นต้องรอแปลโค้ดทั้งหมดก่อนรัน
-   **แก้ไขโค้ดได้ง่าย:**  สามารถแก้ไขโค้ดและรันใหม่ได้ทันที

**ข้อเสียของ Interpreter:**

-   **รันโค้ดช้ากว่า Compiler:**  เนื่องจากต้องแปลโค้ดทีละบรรทัด
-   **กินทรัพยากรระบบมากกว่า Compiler:**  เนื่องจากต้องเก็บโค้ดที่แปลแล้วไว้ในหน่วยความจำ

Programming Language Interpreter เป็นเครื่องมือที่มีประโยชน์สำหรับการพัฒนาโปรแกรม เหมาะสำหรับการพัฒนาโปรแกรมแบบรวดเร็ว โต้ตอบ และแก้ไขง่าย แต่มีข้อเสียคือรันโค้ดช้ากว่า Compiler และกินทรัพยากรระบบมากกว่า

### Python

Python เป็นภาษาโปรแกรมมิ่งที่ถูกคิดค้นโดย Guido van Rossum ที่ Centrum Wiskunde & Informatica (CWI) ในประเทศเนเธอร์แลนด์ ภาษาดังกล่าวเป็น High-level general-purpose programming language ที่เน้นความสามารถในการอ่านโค้ดได้ง่าย นอกจากนี้ Python จะเป็นภาษาที่เป็น dynamically typed และมี garbage-collected รองรับหลาย programming paradigms เช่น OOP และ FP นอกจากนี้ยังมีคุณสมบัติ Battery Included ด้วย Standard Library ที่มีมาให้ใช้งานค่อนข้างกว้าง

ปัจจุบันมี 2 major versions ที่นิยมใช้กันในปัจจุบันได้แก่ 2.X และ 3.X โดยปัจจุบันเวอร์ชั่น 2.7 เป็นเวอร์ชั่นสุดท้ายของ 2.X และไม่ได้รับการ support ต่อแล้ว

#### pip (package manager)

pip หรือที่รู้จักกันใน Python3 ว่า pip3 นั้นเป็น package management system ที่ถูกเขียนด้วย Python และใช้สำหรับการติดตั้งและจัดการ software packages ด้วย Command-line interface ยกตัวอย่างเช่นคำสั่ง `pip install some-package-name` และ `pip uninstall some-packcage-name` จะเป็นการติดตั้งและถอนการติดตั้ง package ที่มีชื่อว่า some-package-name หรือหากต้องการติดตั้ง package ผ่านรายการที่ได้เตรียมอยู่แล้วในไฟล์สามารถใช้คำสั่ง `pip install -r requirements.txt`

#### Python Installation

เกือบทุก Linux distribution นั้นมาพร้อมกับ Python และ pip แล้วโดยสามารถเช็คสถานะการติดตั้งของ Python ได้ผ่านคำสั่ง -`python3 --version` หรือ `python --version`

สำหรับการติดตั้งและอับเดตตัว Python สามารถใช้งานคำสั่ง

1. `sudo apt update` เพื่อทำการอับเดตและตรวจสอบว่ามีเวอร์ชั่นใหม่หรือไม่
2. `sudo apt install python3` เพื่อติดตั้ง Python3 เวอร์ชั่นใหม่ล่าสุด

ในกรณีที่ทราบว่าจะต้องใช้ Python หลายเวอร์ชั่นและอาจจะมีการสลับการไปกันมาระหว่างการใช้งาน สามารถศึกษา [PyEnv](https://github.com/pyenv/pyenv?tab=readme-ov-file#installation) เพิ่มเติมได้ 

### Perl

Perl ถูกพัฒนาโดย Larry Wall ในปี 1987 โดยเป็นภาษา High-level, general purpose, interpreted, dynamic programming language โดยจุดประสงค์หลักสำหรับการพัฒนาเป็น Unix scripting language ที่สามารถทำ report processing ได้ง่ายขึ้น โดยถูกพัฒนาขึ้นด้วยภาษา C

ปัจจุบัน Perl กำลังอยู่ในเวอรชั่นที่ 5 ถูกปล่อยออกมาครั้งแรกในปี 1994 และปัจจุบัน Perl 6 กำลังถูกพัฒนาตั้งแต่ระหว่าง 2000 จนถึงปี 2019 จนกระทั่งได้ถูกเปลี่ยนชื่อมาเป็น Raku โดยปัจจุบันนั้น Perl กับ Raku ที่ได้รับการพัฒนาแยกออกจากกันโดยทีมคนละทีม

#### Perl Installation

ใน Ubuntu เวอร์ชั่นปัจจุบันนั้นได้ preinstalled Perl 5 ติดมากับตัว OS อยู่แล้ว โดยสามารถตรวจสอบสถานะการติดตั้งได้ด้วยคำสั่ง `perl -v`

**ขั้นตอนในการติดตั้ง**
1. ก่อนทำการติดตั้งให้ทำการอับเดต package repository เพื่อให้แน่ใจว่าการติดตั้ง จะติดตั้งเวอร์ชั่นล่าสุด ได้ด้วยคำสั่ง
	```bash
	sudo apt update && sudo apt upgrade -y
	```
2. ถึงแม้ว่า Ubuntu อาจจะมี Perl ติดตั้งมาให้แล้ว แต่เราก็สามารถทำการอับเดตและติดตั้ง Perl เวอร์ชั่นใหม่ล่าสุดได้ด้วยคำสั่ง
	```bash
	sudo apt install perl
	```
	
### Ruby

Ruby เป็นภาษาที่คิดค้นโดย Yukihiro Matsumoto ในปี 1995 โดยเป็นภาษา Interpreted, High-level, general-purpose programming language ที่รองรับหลาย programming paradigms โดยได้ถูกออกแบบมาเพื่อรองรับถึงความเรียบง่ายในการใช้งาน

Matsumoto ได้อธิบายดีไซน์ของ Ruby ไว้ว่าเรียบง่ายเสมือนภาษา Lisp ในแกนหลัก โดยที่มี object system เหมือนภาษา Smalltalk, blocks จาก higher-order functions, และมีฟีเจอร์ที่สามารถนำไปใช้งานในชีวิตจริงได้เหมือน Perl

ปัจจุบันเวอร์ชั่นล่าสุดของ Ruby คือ Ruby 3 โดยที่ Ruby 3.0.0 ได้ถูกปล่อยออกมาครั้งแรกวันคริสต์มาสปี 2020

#### Ruby Installation

สามารถตรวจสอบได้ว่าติดตั้ง Ruby สำเร็จหรือไม่ด้วยคำสั่ง `ruby -v`

Ruby สามารถติดตั้งบนเครื่อง Ubuntu ได้โดยหลายวิธีเช่น การใช้ package manager, การใช้ installer สำหรับการติดตั้ง version เฉพาะที่ต้องการ, การใช้ managers สำหรับการเปลี่ยนเวอร์ชั่นของ Ruby โดยสำหรับเอกสารชุดนี้ จะบอกวิธีการติดตั้งผ่าน package manager เนื่องจากเป็นวิธีที่แนะนำจากบนตัวเว็บไซต์ของ Ruby

1. Ubuntu และ Debian สามารถให้ apt ในการติดตั้ง Ruby On Rails ได้ดังต่อไปนี้ 
	```bash
	sudo apt-get install ruby-full
	``` 
	ในกรณีที่ใช้ CentOS, Fedora หรือ distribution อื่นๆ ที่ใช้ Yum สามารถติดตั้งได้ด้วยคำสั่งดังต่อไปนี้
	```bash
	sudo yum install ruby
	```
#### RubyGems

RubyGems เป็น package manager สำหรับภาษาโปรแกรมมิ่ง Ruby โดยที่ทำหน้าที่เป็นตัวกลางและมาตรฐานของการเผยแพร่และโหลดใช้งาน library ระหว่างกัน

โดยที่ RubyGems ให้การใช้งานผ่าน Command-line tool ที่เรียกว่า Gem ซึ่งสามารถจัดการและ install library (โดยแต่ละ library จะมีชื่อเรียกว่า gem)

#### Ruby Gems Installation

สามารถตรวจสอบสถานะการติดตั้งของ RubyGems ได้ด้วยคำสั่ง `gem -v`

การติดตั้ง RubyGems นั้นจำเป็นที่จะต้องติดตั้ง Ruby ก่อนเรียบร้อย โดยสามารถตรวจสอบสถานะของ Ruby ได้ด้วยคำสั่ง `ruby -v`

1. เนื่องจาก RubyGems นั้นไม่มีอยู่บน apt จึงจำเป็นต้องทำการดาวน์โหลด Installer จาก [Official Website](https://rubygems.org/pages/download) ของ RubyGems หรือได้ด้วยคำสั่ง `wget https://rubygems.org/rubygems/rubygems-3.5.6.tgz` โดยจะเป็นการโหลดเวอร์ชั่นล่าสุด ณ​ เวลาของเอกสารชุดนี้ กรุณาตรวจสอบเวอร์ชั่นล่าสุดในอนาคตผ่าน Official Website ข้างต้น

2. ทำการ unpack/extract ตัว installer .tar file ที่ได้มาจากขั้นตอนที่แล้ว
4. ทำการ cd เข้าไปใน directory ที่ได้
5. ทำการรัน `ruby setup.rb`

#### Ruby on Rails

Ruby on Rails หรือที่รู้จักกันในชื่อของ Rails เป็น Server-side application framework พัฒนาโดย David Heinemeier Hasson เขียนด้วย Ruby ภายใต้ MIT License. โดยที่ Rails นั้นเป็น model-view-controller (MVC) framework ที่รองรับ database, web service และ web page ตั้งแต่แกะกล่อง

Ruby on Rails นั้นถือกำเนิดมาในปี 2005 โดยได้ส่งผลกระทบต่อวงการพัฒนา Web App Development เป็นอย่างมาก ปัจจุบันนั้น Rails อยู่ที่เวอร์ชั่น Rails 7.1 ปล่อยมาในวันที่ 5 ตุลาคม 2023

#### Ruby on Rails Installation

สามารถทำการตรวจสอบสถานะการติดตั้ง Rails ได้ด้วยคำสั่ง `rails --version`

ก่อนการติดตั้ง Rails ให้ทำการตรวจสอบก่อนว่าได้ติดตั้ง Ruby และ RubyGems อยู่บนเครื่องแล้วรึเปล่าได้ด้วยคำสั่ง `ruby --version` และ `gem -v` โดยที่ Rails จะรองรับการทำงานบน Ruby 2.7 ขึ้นไปเท่านั้น

นอกจากนี้ Rails ยังต้องการ SQLite3 database บนเครื่องก่อน โดยที่หลาย OS ที่มีลักษณะเหมือน UNIX นั้นมี version ของ SQLite3 ที่ติดตั้งอยู่ก่อนแล้วพร้อมกับการติดตั้ง Rails โดยสามารถเช็คว่าได้ติดตั้ง SQLite3 เรียบร้อยแล้วด้วยคำสั่งว่า `sqlite3 --version`

1. ทำการติดตั้ง library rails ด้วยคำสั่ง `gem install rails`
 
### Node.js

Node.js ถูกเริ่มต้นพัฒนาโดย Ryan Dahl ในปี 2009 ซึ่งเป็นระยะเวลา 13 ปีหลังจากที่ Javascript เริ่มถูกใช้สำหรับฝั่ง server-side Javascript environment โดยในตอนแรกรองรับการทำงานบน Mac OS X และ Linux เท่านั้น

Node.js เป็นภาษา cross-platform, open-source Javascript Runtime Environment ที่สามารถทำงานได้บน Windows, Linux, Unix, macOS และอื่นๆ โดยที่ Node.js รันต้ว V8 Javascript Engine ของ Google และทำให้ Javascript สามารถทำงานได้นอก Web Browser

Node.js มักถูกใช้ในการทำ server-side scripting โดยจะใช้สร้าง dynamic webpage ก่อนที่จะทำการส่งตัว webpage กลับไปยังฝั่ง client browser นอกจากนี้ Node.js ยังนำเสนอแนวความคิดว่า Javascript Everywhere paradigm ทำให้การสร้าง web-application นั้นสามารถทำได้ภายใต้ภาษาเดียวกันนั้นคือ Javascript

Node.js ใช้ event-driven architecture สำหรับการทำ asynchronous I/O เพื่อเพิ่ม throughput และ scalability ของตัว web application 

#### npm

npm นั้นคือ package manager ของภาษา Javascript โดย npm มาพร้อมกับ command line client หรือที่เรียกกันว่า npm, online database สำหรับ packages ต่างๆ ที่เรียกว่า npm registry 

#### Yarn (package manager)

yarn เป็นหนึ่งใน package manager ที่โด่งดังโดยได้เริ่มพัฒนาครั้งแรกในปี 2016 โดย Sebastian McKenzie จากบริษัท Meta (Facebook) สำหรับ Node.js Javascript Runtime Environment

สามารถตรวจสอบสถานะการติดตั้งของ yarn ได้จากคำสั่ง `yarn --version`

yarn นั้นสามารถถูกติดตั้งได้โดยหลายวิธี ([วิธีอื่นๆ](https://www.hostinger.com/tutorials/how-to-install-yarn)) แต่สำหรับวิธีที่แนะนำนั้นคือการติดตั้งผ่าน npm ด้วยคำสั่ง `sudo npm install --global yarn`

#### Node.js Installation

สามารถตรวจสอบสถานการติดตั้ง Node.js บนเครื่องได้ด้วยคำสั่ง `node -v`

วิธีการติดตั้ง Node.js นั้นมีหลากหลายวิธียกตัวอย่างดังต่อไปนี้

1. ติดตั้งผ่าน apt package manager
	1.1 ทำการอัปเดต local package index ด้วยคำสั่ง
	```bash
	sudo apt update
	```
	1.2 ทำการติดตั้งด้วยคำสั่ง install
	```bash
	sudo apt install nodejs
	```
จากวิธีแรกนั้นเวอร์ชั่นที่ได้ติดตั้งจะเป็นเวอร์ชั่นประมาณ 10.X.X ซึ่งถือว่าเก่าและไม่ได้รับการพัฒนาต่อแล้ว

2. ติดตั้งด้วย Node Version Manager (NVM) **แนะนำ**ให้ติดตั้งด้วยวิธีเนื่องจากว่าจะสามารถเปลี่ยนแปลงเวอร์ชั่นของ Node.js ในภายหลังได้
	2.1 ทำการโหลด NVM ผ่านคำสั่ง curl ว่า
	```bash
	curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh
	```
	ทำการ pipe bash ต่อข้างหลัง หากได้ทำการตรวจสอบ script แล้วว่าปลอดภัยต่อการใช้งานและเข้าใจว่าทำงานอย่างไร จะแก้ไขคำสั่งที่กล่าวข้างต้นเป็น
	```bash
	curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
	```
	2.2 NVM จะทำการติดตั้งตนเองเข้าไปใน .bashrc ให้ทำการ source (execute) ไฟล์ .bashrc ใหม่อีกครั้งโดยใช้คำสั่งได้ว่า หรือทำการ restart/logout
	```
	source ~/.bashrc
	```
	2.3 ทำการดูเวอร์ชั่นของ Node.js ที่สามารถติดตั้งผ่าน NVM ด้วยคำสั่ง `nvm list-remote` 	จากนั้นทำการเลือกฟังก์ชั่นที่ต้องการจะติดตั้งแล้วใช้คำสั่ง install

	```bash
	nvm install v14.10.0
	```

## อ้างอิง References

- **The Linux Documentation Project:** 
 [https://www.tldp.org/LDP/abs/html/](https://www.tldp.org/LDP/abs/html/)
- **Bash Reference Manual:**  [https://www.gnu.org/software/bash/manual/html_node/index.html](https://www.gnu.org/software/bash/manual/html_node/index.html)
-  **Zsh Documentation:** 
[https://zsh.sourceforge.io/Doc/](https://zsh.sourceforge.io/Doc/)
- **Techadmin** 
[https://tecadmin.net/difference-between-sh-and-bash/#:~:text=SH%20is%20a%20classic%2C%20minimalistic,a%20proficient%20shell%20script%20writer.](https://tecadmin.net/difference-between-sh-and-bash/#:~:text=SH%20is%20a%20classic%2C%20minimalistic,a%20proficient%20shell%20script%20writer.)
- **Z shell Wikipedia**
[https://en.wikipedia.org/wiki/Z_shell](https://en.wikipedia.org/wiki/Z_shell)
- **Zsh vs. Bash Scripting. What’s the Difference?**
[https://www.makeuseof.com/zsh-bash-scripting-difference/#:~:text=The%20main%20difference%20is%20that,Bash%20only%20supports%20string%20keys.](https://www.makeuseof.com/zsh-bash-scripting-difference/#:~:text=The%20main%20difference%20is%20that,Bash%20only%20supports%20string%20keys.)
-   **Interpreter Wikipedia:**  
[https://simple.wikipedia.org/wiki/Interpreter](https://simple.wikipedia.org/wiki/Interpreter)
-   **GeeksforGeeks:** 
[https://www.geeksforgeeks.org/difference-between-compiler-and-interpreter/](https://www.geeksforgeeks.org/difference-between-compiler-and-interpreter/)
-   **Tutorialspoint:**  
[https://www.tutorialspoint.com/ansi_c/c_introduction.htm](https://www.tutorialspoint.com/ansi_c/c_introduction.htm)
-   **Python:**  
[https://docs.python.org/](https://docs.python.org/)
- **Python Wikipedia**
[https://en.wikipedia.org/wiki/Python_(programming_language)](https://en.wikipedia.org/wiki/Python_(programming_language))
- **Perl Wikipedia** 
[https://en.wikipedia.org/wiki/Perl](https://en.wikipedia.org/wiki/Perl)
- **pip (package manager)**
[https://en.wikipedia.org/wiki/Pip_(package_manager)](https://en.wikipedia.org/wiki/Pip_(package_manager))
-   **JavaScript:**
[https://developer.mozilla.org/en-US/docs/Web/JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
-   **Ruby:**  
[https://ruby-doc.org/](https://ruby-doc.org/)
-   **PHP:**
[https://www.php.net/manual/en/index.php](https://www.php.net/manual/en/index.php)
-   **Perl:** 
[https://perldoc.perl.org/](https://perldoc.perl.org/)
- **Web Hosting Geeks**
[https://webhostinggeeks.com/howto/how-to-install-perl-on-ubuntu/](https://webhostinggeeks.com/howto/how-to-install-perl-on-ubuntu/)
- **RubyGems**
[https://rubygems.org/](https://rubygems.org/)
- **RubyGems Wikipedia**
[https://en.wikipedia.org/wiki/RubyGems](https://en.wikipedia.org/wiki/RubyGems)
- **LinuxHint** 
[https://linuxhint.com/install-rubygems-ubuntu/](https://linuxhint.com/install-rubygems-ubuntu/)
- **Ruby on Rails Wikipedia** 
[https://en.wikipedia.org/wiki/Ruby_on_Rails](https://en.wikipedia.org/wiki/Ruby_on_Rails)
- **Node.js Wikipedia**
[https://en.wikipedia.org/wiki/Node.js](https://en.wikipedia.org/wiki/Node.js)
- **npm Wikipedia**
[https://en.wikipedia.org/wiki/Npm](https://en.wikipedia.org/wiki/Npm)
- **Yarn (package manager) Wikipedia**
[https://en.wikipedia.org/wiki/Yarn_(package_manager)](https://en.wikipedia.org/wiki/Yarn_(package_manager))
- **Yarnpkg Webpage**
[https://yarnpkg.com/getting-started/install](https://yarnpkg.com/getting-started/install)
- **DigitalOcean Node.js**
[https://www.digitalocean.com/community/tutorial-series/how-to-install-node-js-and-create-a-local-development-environment](https://www.digitalocean.com/community/tutorial-series/how-to-install-node-js-and-create-a-local-development-environment)
