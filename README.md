# Project 7 - WordPress Pentesting
Time spent: **6** hours spent in total

> Objective: Find, analyze, recreate, and document **three vulnerabilities** affecting an old version of WordPress

## Pentesting Report
1. (Required) XSS in URL Embeds
  - [ ] Summary: 
    - Vulnerability types: Stored XSS in WP Core
    - Tested in version: 4.2
    - Fixed in version: 4.2.13
  - [ ] GIF Walkthrough: <img src="pro7_1.gif" width="800">
  - [ ] Steps to recreate: Open up a new post and add an embedded YouTube video URL. In the URL, add an XSS at the end. For this example, "svg onload=alert(1)" was used to show a pop-up alert everytime the video would load. 
  
  - [ ] Affected source code:
    - [Link 1](https://github.com/WordPress/WordPress/commit/419c8d97ce8df7d5004ee0b566bc5e095f0a6ca8)
    
2. (Required) XSS in Embed YouTube URLs
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.13
  - [ ] GIF Walkthrough: <img src="pro7_2.gif" width="800">
  - [ ] Steps to recreate: Open up a new post, and insert the embedded link for a YouTube video. At the end of the main embedded video statement, add an alert whenever the video loads. In this case, "onload=alert(123456789)" was the alert used. 
  - [ ] Affected source code:
    - [Link 2](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)

3. (Required) Vulnerability Name or ID
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

    Copyright [2018] [Thomas Lu]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
