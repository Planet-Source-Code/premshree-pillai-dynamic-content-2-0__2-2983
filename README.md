<div align="center">

## Dynamic Content 2\.0


</div>

### Description

This JavaScript displays different content for different links on the same area, dynamically.
 
### More Info
 
This JavaScript displays different content for different links on the same area, dynamically.

You can display any content in the area. The function is called like this »

<a href="javascript:void(0);" onClick="javascript:showContent('<font face=verdana,arial,helvetica>This is Content 1</font>');"><font face="verdana,arial,helvetica" color="#CC0000" size="-1"><b>Content 1</b></font></a>

The content marked bold above is the content that you want to display when a link is clicked. You can include <HTML> tags also. So you can even include images.

This version (v 2.0) supports IE, NS4, NS6.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Premshree Pillai](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/premshree-pillai.md)
**Level**          |Intermediate
**User Rating**    |4.7 (14 globes from 3 users)
**Compatibility**  |
**Category**       |[Layers](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/layers__2-78.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/premshree-pillai-dynamic-content-2-0__2-2983/archive/master.zip)





### Source Code

```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN">
<html>
<head>
<title>Dynamic Content 2.0</title>
<style type="text/css">
.link{font-family:verdana,arial,helvetica; font-size:8pt; color:#404040; font-weight:normal; text-decoration:underline}
.link:hover{font-family:verdana,arial,helvetica; font-size:8pt; color:#CC0000; font-weight:normal; text-decoration:underline}
.header{font-family:verdana,arial,helvetica; font-size:22pt; color:#404040; font-weight:bold; text-decoration:none}
</style>
</head>
<body bgcolor="#FFFFFF">
<center><span class="header">Dynamic Content 2.0</span></center><br>
<!-------------------------------------------------------------------------------------->
<!--BEGIN DYNAMIC CONTENT 2.0-->
<script language="JavaScript1.2">
//-----------------------------------------------
// Dynamic Content 2.0             |
// Now supports IE, NS4, NS6          |
// (c) 2002 Premshree Pillai          |
// Web : http://www.qiksearch.com        |
// E-mail :premshree@hotmail.com        |
// Use freely as long as this message is intact |
//-----------------------------------------------
// Location of script : http://www.qiksearch.com/javascripts/dynamic-content20.htm
var ie4=document.all&&navigator.userAgent.indexOf("Opera")==-1;
var ns6=document.getElementById&&navigator.userAgent.indexOf("Opera")==-1;
var ns4=document.layers;
function showContent(content)
{
 if(ie4)
 {
 showContentObj=document.all.qiksearch_div;
 }
 if(ns6)
 {
 showContentObj=document.getElementById("qiksearch_div");
 }
 if(ie4||ns6)
 {
 if(showContentObj.innerHTML!=content)
 {
  showContentObj.innerHTML=content;
 }
 else
 {
  showContentObj.innerHTML="";
 }
 }
 if(ns4)
 {
 document.nsdiv.document.write(content);
 document.nsdiv.document.close();
 }
}
</script>
<center>
<a href="javascript:void(0);" onClick="javascript:showContent('<font face=verdana,arial,helvetica>This is Content 1</font>');"><font face="verdana,arial,helvetica" color="#CC0000" size="-1"><b>Content 1</b></font></a> | <a href="javascript:void(0);" onClick="javascript:showContent('<font face=verdana,arial,helvetica>This is Content 2</font>');"><font face="verdana,arial,helvetica" color="#CC0000" size="-1"><b>Content 2</b></font></a> | <a href="javascript:void(0);" onClick="javascript:showContent('<font face=verdana,arial,helvetica>This is Content 3</font>');"><font face="verdana,arial,helvetica" color="#CC0000" size="-1"><b>Content 3</b></font></a>
<br><br><layer id="nsdiv" left="310"></layer>
<div id="qiksearch_div"></div></center>
<!--END DYNAMIC CONTENT 2.0-->
<!-------------------------------------------------------------------------------------->
<br><table align="center" width="400" cellspacing="0"><tr><td>
<font face="verdana,arial,helvetica" size="-1" color="#404040">
This JavaScript displays different content for different links on the same area, dynamically.
<br><br>
You can display any content in the area. The function is called like this &raquo;
<br><br><font face="courier">&lt;a href="javascript:void(0);" onClick="javascript:showContent('<b>&lt;font face=verdana,arial,helvetica&gt;This is Content 1&lt;/font&gt;</b>');"&gt;&lt;font face="verdana,arial,helvetica" color="#CC0000" size="-1"&gt;&lt;b&gt;Content 1&lt;/b&gt;&lt;/font&gt;&lt;/a&gt;</font>
<br><br>The content marked bold above is the content that you want to display when a link is clicked. You can include &lt;HTML&gt; tags also. So you can even include images.
<br><br>This version (<b>v 2.0</b>) supports IE, NS4, NS6.
</font>
<hr width="100%" style="height:1px; color:#CC0000">
</td></tr></table>
<center><a href="http://www.qiksearch.com" class="link">&#169 2002 Premshree Pillai. All rights reserved.</a></center>
</body>
</html>
```

