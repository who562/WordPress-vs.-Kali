# Project 7 - WordPress Pentesting

Time spent: 5 hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

### 1. (Required) Wordpress < 5.1.1/ CVE-2019-9787: Cross-Site Request Forgery (CSRF)
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.0
    - Fixed in version: 5.1.1
  - [X] GIF Walkthrough: 
       <img src=XSS.gif />
  - [X] Steps to recreate: 
     Login and enter a page
             <img src=xss1.jpg />
             
     Enter the script in the comment section
             <img src=xss2.jpg />
             
      Post the comment and enjoy 
             <img src=xss3.jpg />
  - [X] Affected source code:
           <img src=xsscode.jpg />
### 2. (Required) User Enumeration
  - [X] Summary: 
    - Vulnerability types:User Enumeration
    - Tested in version:4.0
    - Fixed in version: 
  - [X] GIF Walkthrough: 
           <img src=https://github.com/who909/WordPress-vs.-Kali/blob/baa3924833f64f5de23616c05b5bb381471c76ae/User%20Enumeration.gif />
  - [X] Steps to recreate: 
             Enter the login page.
             <img src=https://github.com/who909/WordPress-vs.-Kali/blob/b1f11febafbe1c45d0433f56aa907104ca23e126/User%20Enumeration.jpg/>
        
      enter admin as username and a random password.
        <img src=https://github.com/who909/WordPress-vs.-Kali/blob/b1f11febafbe1c45d0433f56aa907104ca23e126/User%20Enumeration2.jpg/>
        
        
      If the user exists, WordPress word gives an error message for an incorrect password. 
       <img src=https://github.com/who909/WordPress-vs.-Kali/blob/b1f11febafbe1c45d0433f56aa907104ca23e126/User%20Enumeration3.jpg/>
       
       If the user does not exist, WordPress word gives an error message for an invalid username.
         <img src=https://github.com/who909/WordPress-vs.-Kali/blob/b1f11febafbe1c45d0433f56aa907104ca23e126/User%20Enumeration4.jpg/>
### 3. (Required) XSS media
  - [X] Summary: XSS media
    - Vulnerability types:XSS
    - Tested in version:4.0
    - Fixed in version: 5.1.2
  - [X] GIF Walkthrough: 
   <img src=XSSmed.gif />
   
  - [X] Steps to recreate:Enter the admin console, create or edit a page.
        <img src=xssmed1.jpg />
        
       click add media
       <img src=xssmed2.jpg />
        
       Choice an image and add the XSS script to the description. Then, change the link page to attachment page.
       <img src=xssmed3.jpg />
       
       Post and then view the page. click the image. 
         <img src=xssmed4.jpg />
       
       Done
        <img src=xssmed5.jpg />
  - [X] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)


## Assets

List any additional assets, such as scripts or files

XSS cheatsheet(https://cheatsheetseries.owasp.org/cheatsheets/XSS_Filter_Evasion_Cheat_Sheet.html/)

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [Screentogif](https://www.screentogif.com/).

## Notes

Describe any challenges encountered while doing the work

- Bitdefender and Microsoft antivirus were blocking payloads.

## License

    Copyright [2021] [Alejandro Bravo]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
