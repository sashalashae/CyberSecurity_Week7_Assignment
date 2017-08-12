# CyberSecurity_Week7_Assignment

# Project 7 - WordPress Pentesting

Time spent: 2 hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1\. [x]  (Required) WordPress <= 4.2 - Unauthenticated Stored Cross-Site Scripting (XSS)
* [x] Summary: 
- Vulnerability types: XSS Injection
- Tested in version: Wordpress 4.2
- Fixed in version: Wordpress 4.2
* [x] GIF Walkthrough: 
<img src='http://i.imgur.com/c63n0ti.gif' />
* [x] Steps to recreate: 
Go to the comments section of the page.  Enter in <script>while(1){alert(document.cookie);}</script> in the comments box.  Warning once you click submit, the page will refresh and you will have an infinite amount of alert messages.  After you are done with this vulnerability, to end the message, go to the info page and delete the comment.

GIF created with [LiceCap](http://www.cockos.com/licecap/).

## Notes


## License

Copyright [2017] [Sasha Morgan]

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
