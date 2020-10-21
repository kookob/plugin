# Toolset

## Introduction
Toolset is a plugin for the IntelliJ platform, which contains a variety of toolset to facilitate the coding of developers and improve development efficiency.

## Features
Contains multiple Tabs, each Tab contains some sub-tabs, and each tab provides corresponding functions.  

*   **Convert**
    *   Common: Base64, Hex, URI, URIComponent, Unicode
    *   Decimal: Hex conversion, JavaScript execute
    *   Json: Format, Quote Parse, Key:Value, XML, Excel
    *   Sort: Sort Lines, Reverse Lines, Remove Duplicate Lines, Sort and Remove Duplicate, Remove Line Number
    *   Time: Timestamp, Calculate Difference
    *   Color: Conversion, Picker
    *   ImageBase64: image ⇄ base64
*   **Cron**: Cron Expression Generator & Explainer
*   **Encrypt**
    *   Digest: MD5,SHA1,SHA256,SHA384,SHA512,HmacMD5,HmacSHA1,HmacSHA256,HmacSHA384,HmacSHA512
    *   Asymmetric: RSA
*   **Generate**
    *   UUID
    *   Password
    *   File Verification: MD5,SHA1,CRC32
*   **HttpServer**: Simple Http Server
*   **Note**: Temporary notebook
*   **Pomodoro**: Stay focused, be productive, track everything.
*   **Regex**
    *   Tester: Regexp Tester
    *   Extract
    *   Replace: Right-Click Menu
*   **Symbols**
    *   Ascii: ASCII, Html Escape
    *   KeyCode
    *   Symbols: Arrows, Alphabet, Currency, Geometric, Miscellaneous Symbols...
*   **SwitchHosts**: Switch and Manager hosts
*   **Terminal**
    *   common
    *   cat
    *   curl
    *   file
    *   apt
    *   rpt
    *   yum
    *   mysqldump

---
  
Right Click Menu String Manipulation

*   **Convert**
    *   '.\*' ⇄ \`.\*\`
    *   '.\*' ⇄ ".\*"
*   **Encode/Decode**
    *   Base64 Encode
    *   Base64 Decode
    *   Hex Encode
    *   Hex Decode
    *   Html Encode
    *   Html Decode
    *   Unicode Encode
    *   Unicode Encode
    *   URI Encode
    *   URI Decode
*   **Lines**
    *   Sort Lines
    *   Remove Duplicate Lines
    *   Sort And Remove Duplicate Lines
    *   Copy Cursor Line
*   **Switch To**
    *   foo\_bar
    *   fooBar
    *   FooBar
    *   FOO\_BAR
*   **Trim**
    *   Trim
    *   Trim Start
    *   Trim End
*   **Regex Replace**

## Pictures
![](https://plugins.jetbrains.com/files/14384/339-page/image244.png)  
Common is some commonly used encoding and decoding.  

![](https://plugins.jetbrains.com/files/14384/339-page/image245.png)  
Decimal is a number-related processing, such as the most commonly used decimal conversion.  
The input box on the left can execute simple one-line JavaScript code, such as: numeric operations, character processing, date operations, and so on.  

![](https://plugins.jetbrains.com/files/14384/339-page/image246.png)  
Json tags can handle some formatting, remove or restore quotation marks, convert to Key:Value format, convert between Json and XML, and convert between Json array and Excel.  

![](https://plugins.jetbrains.com/files/14384/339-page/image247.png)  
Sorting is relatively simple. Sort multiple lines of text, reverse order, remove duplicate lines, or remove the first number of lines (for example, sometimes when copying code, you need to remove useless line numbers)  

![](https://plugins.jetbrains.com/files/14384/339-page/image248.png)  
Time: A tool for calculating time, such as time format conversion, which calculates that 100 days is approximately equal to several hours, and the calculation of two time differences.  
Note that the arrow position above can be clicked to switch the time on the left and right.  
Double click start time and end time to get the current time directly  

![](https://plugins.jetbrains.com/files/14384/339-page/image249.png)  
Color: color value and format conversion  

![](https://plugins.jetbrains.com/files/14384/339-page/image250.png)  
To convert between Image and Base64, you can directly drag and drop image files in the left window.  

![](https://plugins.jetbrains.com/files/14384/339-page/image251.png)  
Cron: Timer expression generation and de-analysis, friends who often need to write timers, with this function, it is really convenient.  

![](https://plugins.jetbrains.com/files/14384/339-page/image252.png)  
Commonly used encryption processing, the above Loop can loop the calculation results.  
Asymmetric currently only implements the RSA algorithm. Pay attention to the arrow buttons for easy operation. There will be energy to implement more algorithms in the future.  
  
![](https://plugins.jetbrains.com/files/14384/339-page/image253.png)  
The function of Generate Tab is relatively simple. It implements a password generator, UUID generation, and calculations of MD5 and SHA1 of files. When File Verification is used, you can directly drag and drop files.  

![](https://plugins.jetbrains.com/files/14384/339-page/image254.png)  
HttpServer: Simple Http service provided. After clicking the Start button, you can directly access the local corresponding address: http://localhost:8888/  
Pay attention to the configuration path and port, the position of the red arrow, you can directly use the default browser to open.  

![](https://plugins.jetbrains.com/files/14384/339-page/image255.png)  
Note: Some simple and temporary text records, the file is saved in the file address in the red box in the upper left corner in real time, and the Statistics button on the upper right can count the relevant number of characters.  

![](https://plugins.jetbrains.com/files/14384/339-page/image256.png)  
Pomodoro: Pomodoro method, depending on personal circumstances, may not be used by many people, let’s talk about the following hidden functions:  
Above the 25:00 number, the mouse wheel can adjust the number of minutes to count down, double-click to restore to 25 minutes.  
The text entered in the window needs to be clicked on the Save button to be saved to a temporary file, and will not be lost next time you restart the IDE.  

![](https://plugins.jetbrains.com/files/14384/339-page/image257.png)  
![](https://plugins.jetbrains.com/files/14384/339-page/image258.png)  
![](https://plugins.jetbrains.com/files/14384/339-page/image259.png)  
![](https://plugins.jetbrains.com/files/14384/339-page/image260.png)  
![](https://plugins.jetbrains.com/files/14384/339-page/image261.png)  
![](https://plugins.jetbrains.com/files/14384/339-page/image262.png)  

## Right-Click Menu
![](https://plugins.jetbrains.com/files/14384/339-page/image263.png)  
- Convert: Single quotation marks, double quotation marks, `signs are mutually converted  
- Encode/Decode: Right-click menu implementation of Convert window  
- Switch To: Conversion before Luofeng string format  
- Trim: Remove leading and trailing spaces  
- Regex Replace: Right-click menu operation of regular window configuration  

## Settings
![](https://plugins.jetbrains.com/files/14384/339-page/image264.png)  
Disable unnecessary functions and enable only frequently used functions to make the Toolset window more concise  

## Planning
At present, the plug-in has so many functions, but I still want to continue to add in the functions that can improve the efficiency of development in the usual development process, so the functions will only increase, if there are too many friends, you can disable it by yourself. When disabled, it will not take up any performance.  
I will continue to develop and improve when I have time in the follow-up. At present, some functions are already planned:  
- [ ] Code formatting in various languages
- [ ] SQL processing related functions
- [ ] Some more general documents, such as regular expressions
- [ ] Continue to integrate more commonly used commands of general software in Terminal, such as: git, node, pm2, etc., which need time to organize
- [ ] Picture related processing
- [ ] QR code generation and recognition

To be continue...

## Download
[Toolset](https://plugins.jetbrains.com/plugin/14384-toolset/versions)  

## Price
`$5/year`

## Plugins
* [MyBatis Log Plugin](https://plugins.jetbrains.com/plugin/13905-mybatis-log-plugin) 
* [JPA SQL](https://plugins.jetbrains.com/plugin/15242-jpa-sql) 
* [Smart Jump](https://plugins.jetbrains.com/plugin/14053-smart-jump) 
* [Smart Search](https://plugins.jetbrains.com/plugin/14615-smart-search)
* [Toolset](https://plugins.jetbrains.com/plugin/14384-toolset) 
