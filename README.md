# CyberSecurity_Week7_Assignment

# Project 7 - WordPress Pentesting

Time spent: 2 hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1\. [x]  (Required) WordPress <= 4.2 - Unauthenticated Stored Cross-Site Scripting (XSS)
- [x] Summary: 
- Vulnerability types: XSS
- Tested in version: 4.2
- Fixed in version: 4.2
- [x] GIF Walkthrough:<img src='http://i.imgur.com/jeGAJgF.gif' title='GIF Walkthrough' width='' alt='GIF Walkthrough' /> 
- [x] Steps to recreate: Go to the comments section of the page.  Enter in <script>while(1){alert(document.cookie);}</script> in the comments box.  Warning once you click submit, the page will refresh and you will have an infinite amount of alert messages.  After you are done with this vulnerability, to end the message, go to the info page and delete the comment.
- [x] Affected source code:
- [Link 1](https://github.com/WordPress/WordPress/commit/419c8d97ce8df7d5004ee0b566bc5e095f0a6ca8)

2\. [x]  (Required) WordPress 3.6.0-4.7.2 - Authenticated Cross-Site Scripting (XSS) via Media File Metadata
- [x] Summary: 
- Vulnerability types: XSS Injection
- Tested in version: 4.1.1
- Fixed in version: 4.2.13
- [x] GIF Walkthrough:<img src='http://i.imgur.com/DfD3ETz.gif' title='GIF Walkthrough' width='' alt='GIF Walkthrough' /> 
- [x] Steps to recreate: 
    - Add three or more media files to your wordpress library, insert "Let it go <noscript/><script>alert(document.cookie);</script>" into the description of the media file.
    - Create a new post and add the media file to the post as an audio playlist.
    - You should recieve an error message when you try to create the playlist.
- [x] Affected source code:
- [Link 2](https://github.com/WordPress/WordPress/commit/28f838ca3ee205b6f39cd2bf23eb4e5f52796bd7)




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
