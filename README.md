# The PHP version of Feifei Movie and Television System V2.7.130201 has a storage type XSS vulnerability

Feifei V2.7.130201 installation package:https://www.tongyixiazai.com/soft/10001228.html

Recurrence environment:

Windows 10

Phpstudy

Vulnerability description：

The vulnerability exists in \Public\system\slide_add.htmlfiles that are not filtered for any special characters during the addition process, resulting in a storage based XSS vulnerability.

Vulnerability recurrence:

Extension tool - Add slide introduction parameter input script for homepage slide<style onload=alert(1)>，There is a storage type XSS vulnerability, as shown in the figure.

<img width="416" alt="image" src="https://user-images.githubusercontent.com/59866013/226814503-04356893-de7b-47cd-b366-04a15aaef3e3.png">

<img width="416" alt="image" src="https://user-images.githubusercontent.com/59866013/226814600-e8c4fad7-1ed2-47a7-b834-ba33cc1cb36a.png">

![Uploading image.png…]()

As can be seen from the following figure，in the file\Public\system\slide_add.html，during the process of adding the homepage slide, parameters are brought into the database for update without any processing

