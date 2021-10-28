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
     login and enter a page
             <img src=xss1.jpg />
             
     enter the script in the comment section
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
             <img src=User Enumeration.jpg/>
        
      enter admin as username and a random password.
        <img src=User Enumeration2.jpg/>
        
        
      if the user exist, Wordpress word give an error message for incorrect password.
       <img src=User Enumeration3.jpg/>
       
       if the user does not exist, Wordpress word give an error message for invalid username.
         <img src=User Enumeration4.jpg/>
### 3. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)


## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

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
