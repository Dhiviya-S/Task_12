**Dynamic XPath on [https://www.guvi.in/](https://www.guvi.in/)**

**XPATH (XML Path Language):**  
	XPath is a language or syntax to identify any web element using XPath expression. There are two types of XPath:

	* Absolute XPath  
  	* Relative XPath

**Syntax of XPath:**   
	//tagname\[@attribute='value'\]  
		(or)  
	//\*\[@attribute='value'\]

**Absolute XPath(/):**  
	Absolute XPath identifies web elements starting from the root element. This begins with  /(single slash) symbol.  
**Eg:**/html/body/div\[1\]/main/div/div\[1\]/section\[2\]/div/div\[1\]/div/div\[1\]/div/div/input\[1\]

**Relative Xpath(//):**  
	Relative Xpath (or) Dynamic XPath identifies the exact web element but not from the root element. This is a robust and flexible one.This begins with  //(double slash) symbol.Even if any web element changes it is not impacted.  
**Eg:**//input\[@name='email'\]

**Xpath Axes:**   
	**Syntax:**//tagname\[@attribute='value'\]/axes::\*  (\* means ALL)

**Axes-**parent,child,ancestor,descendant,following,preceding,following-sibling,preceding-sibling,self.

	Eg:  //p\[@id="liveclasseslink"\]/parent::div

**This represents the LIVE Classes menu where // is Relative XPath, p=tagname, id=attribute, liveclasseslink=value and parent is keyword, div is parent tag for LIVE Classes.**

**Dynamic XPath on [https://www.guvi.in/](https://www.guvi.in/)**

**Courses:**(//a\[@href="/courses/"\])\[1\]  
“a” is tag name and “href” is attribute and \[1\] represents indexing to select “Courses”

| AXES | Xpath |
| ----- | ----- |
| Parent | (//a\[@href="/courses/"\])\[1\]/parent::div Only one parent for the element “div” |
| First Child  | No child element under “Courses” menu  |
| Second Sibling  | (//a\[@href="/courses/"\])\[1\]/following-sibling::\*\[2\] All siblings are of same name so used indexing \[2\] |
| Ancestor  | (//a\[@href="/courses/"\])\[1\]/ancestor::\*  |
| Following-sibling  | (//a\[@href="/courses/"\])\[1\]/following-sibling::\*  |
| Preceding  | (//a\[@href="/courses/"\])\[1\]/preceding::\* |

**LIVE Classes:** //p\[@id="liveclasseslink"\]  
“p” is tag name and attribute is “id”and its value is liveclasseslink

| AXES | Xpath |
| ----- | ----- |
| Parent | //p\[@id="liveclasseslink"\]/parent::div |
| First Child  | No child element under LIVE Classes menu  |
| Second Sibling  | //p\[@id="liveclasseslink"\]/following-sibling::div |
| Ancestor  | //p\[@id="liveclasseslink"\]/ancestor::\* |
| Following-sibling  | //p\[@id="liveclasseslink"\]/following-sibling::\* |
| Preceding  | //p\[@id="liveclasseslink"\]/preceding::\* |

**Practice:**//p\[@id="practiceslink"\]  
“p” is tag name and attribute is “id” and its value is practiceslink

| AXES | Xpath |
| ----- | ----- |
| Parent | //p\[@id="practiceslink"\]/parent::div |
| First Child  | No child element under Practice menu |
| Second Sibling  | //p\[@id="practiceslink"\]/following-sibling::div |
| Ancestor  | //p\[@id="practiceslink"\]/ancestor::\* |
| Following-sibling  | //p\[@id="practiceslink"\]/following-sibling::\* |
| Preceding  | //p\[@id="practiceslink"\]/preceding::\* |

**Resources:** //p\[@id="resourceslink"\]  
“p” is tag name and attribute is “id” and its value is resourceslink

| AXES | Xpath |
| ----- | ----- |
| Parent | //p\[@id="resourceslink"\]/parent::div |
| First Child  | No child element under Resources menu |
| Second Sibling  | //p\[@id="resourceslink"\]/following-sibling::div |
| Ancestor  | //p\[@id="resourceslink"\]/ancestor::\* |
| Following-sibling  | //p\[@id="resourceslink"\]/following-sibling::\* |
| Preceding  | //p\[@id="resourceslink"\]/preceding::\* |

**Products:** //p\[@id="solutionslink"\]  
“p” is tag name and attribute is “id” and its value is solutionslink

| AXES | Xpath |
| ----- | ----- |
| Parent | //p\[@id="solutionslink"\]/parent::div |
| First Child  | No child element under Products menu |
| Second Sibling  | //p\[@id="solutionslink"\]/following-sibling::div |
| Ancestor  | //p\[@id="solutionslink"\]/ancestor::\* |
| Following-sibling  | //p\[@id="solutionslink"\]/following-sibling::\* |
| Preceding  | //p\[@id="solutionslink"\]/preceding::\* |

**Login:** (//a\[@href="/sign-in/"\])\[2\]  (or)  //a\[@id='login-btn'\]    
“a” is tag name and “href” is attribute and \[2\] represents indexing to select “Login”

| AXES | Xpath |
| ----- | ----- |
| Parent | (//a\[@href="/sign-in/"\])\[2\]/parent::div |
| First Child  | No child element under Login menu |
| Second Sibling  | **No second sibling under Login menu**  |
| Ancestor  | (//a\[@href="/sign-in/"\])\[2\]/ancestor::\* |
| Following-sibling  | **No following sibling under Login menu**  |
| Preceding  | (//a\[@href="/sign-in/"\])\[2\]/preceding::\* |

**Sign up:** (//a\[@href="/register/"\])\[2\] (or)  //a\[text()=”Sign up”\]  
“a” is tag name and “href” is attribute and \[2\] represents indexing to select “Sign up”

| AXES | Xpath |
| ----- | ----- |
| Parent | (//a\[@href="/register/"\])\[2\]/parent::div |
| First Child  | No child element under Sign up icon |
| Second Sibling  | **No second sibling under Sign up menu**  |
| Ancestor  | (//a\[@href="/register/"\])\[2\]/ancestor::\* |
| Following-sibling  | **No following sibling under Sign up menu** |
| Preceding  | (//a\[@href="/register/"\])\[2\]/preceding::\* |

