![smart-jump](https://img.shields.io/jetbrains/plugin/v/14053-smart-jump?label=version&style=flat-square)
[![mybatis-log-plugin](https://img.shields.io/jetbrains/plugin/d/14053-smart-jump?style=flat-square)](https://plugins.jetbrains.com/plugin/14053-smart-jump/versions)
![](https://visitor-badge.glitch.me/badge?page_id=smart-jump)

# Smart Jump
## Introduction
One supports various navigation jumps, makes up for scenarios where the IDE does not provide navigation, and improves development efficiency.  

![](https://plugins.jetbrains.com/files/14053/341-page/image265.png)  

## Support Scene
- Java Method ➔ MyBatis Xml
- MyBatis Xml ➔ Java Method
- Html ➔ JS/CSS file
- Html ➔ JS function
- Vue event ➔ JS function
- JS file ➔ Java Controller RequestMapping
- Eggjs jump

The above support scenarios can be configured through switches and are valid for the project. The default is to enable all. If the project has unnecessary jumps, you can uncheck it.  
If there is no corresponding extension file, whether it is enabled or not has no effect on performance.  
File | Settings | Other Settings | Smart Jump  
![](https://plugins.jetbrains.com/files/14053/341-page/image266.png)  

## Navigation jump
At present, the plugin implements three ways to trigger navigation jumps to facilitate various operating habits of different users.  
- Click the jump icon (little rabbit) on the left side of the code
- Right-click menu to select Smart Jump to achieve jump
- Keyboard shortcut Alt+J (customizable)
Most scenes support the three jump methods, and some scene jumps only support the right-click menu and shortcut keys, such as the Controller RequestMapping method of js file jumping to Java. Because parsing the entire file will consume a certain amount of performance, only the selected text or Locate the line where the mouse is located, then analyze the jump target.  

## Supplement
For some not so intuitive jump functions of the plug-in, here is a supplement:  
MyBatis Xml jumps to Java Method. If you are using a shortcut key or the right mouse button, you do not need to select the text, and the mouse is positioned inside the sql statement to achieve the jump.  
The js file jumps to the Java Request Mapping method. If the line where the mouse is located and the text is not selected, the URL link matching the line will be automatically detected. If there are multiple jump addresses in the line, it is recommended to select the text to be jumped and then trigger the jump.  
If the Java project uses the maven framework, the mouse is positioned inside the dependency, and you can use the shortcut key or the right mouse button to jump to the warehouse address corresponding to the https://mvnrepository.com/ website.  

## Pictures
![](https://plugins.jetbrains.com/files/14053/341-page/image266.png)  
![](https://plugins.jetbrains.com/files/14053/341-page/image267.png)  
![](https://plugins.jetbrains.com/files/14053/341-page/image268.png)  
![](https://plugins.jetbrains.com/files/14053/341-page/image269.png)  
![](https://plugins.jetbrains.com/files/14053/341-page/image270.png)  
![](https://plugins.jetbrains.com/files/14053/341-page/image271.png)  

## Planning
Because the number of development languages and frameworks I have contact with is limited, I can’t access all the scenes that need to be jumped, so if you encounter other languages or frameworks that need to be supported by the plugin, please feel free to contact me, thank you.  
More jump scenarios will be supported in the future.  

## Download
[Smart Jump](https://plugins.jetbrains.com/plugin/14053-smart-jump/versions)  

## Price
`$5/year`

## Plugins
* [MyBatis Log Plugin](https://plugins.jetbrains.com/plugin/13905-mybatis-log-plugin) 
* [JPA SQL](https://plugins.jetbrains.com/plugin/15242-jpa-sql) 
* [Smart Jump](https://plugins.jetbrains.com/plugin/14053-smart-jump) 
* [Smart Search](https://plugins.jetbrains.com/plugin/14615-smart-search)
* [Toolset](https://plugins.jetbrains.com/plugin/14384-toolset) 
