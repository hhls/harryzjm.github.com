---  
layout: post  
title: 正则数字  
category: Command  
tags: 正则  
keywords: 正则  
description: 
---  

### 数字  
	^[0-9]*$  

### n位的数字  
	^d{n}$  

### 至少n位的数字  
	^d{n,}$  

### m-n位的数字  
	^d{m,n}$  

### 零和非零开头的数字  
	^(0|[1-9][0-9]*)$  

### 非零开头的最多带两位小数的数字  
	^([1-9][0-9]*)+(.[0-9]{1,2})?$  

### 带1-2位小数的正数或负数  
	^(-)?d+(.d{1,2})?$  

### 正数、负数、和小数  
	^(-|+)?d+(.d+)?$  

### 有两位小数的正实数  
	^[0-9]+(.[0-9]{2})?$  

### 有1~3位小数的正实数  
	^[0-9]+(.[0-9]{1,3})?$  

### 非零的正整数  
	^[1-9]d*$  
	^([1-9][0-9]*){1,3}$  
	^+?[1-9][0-9]*$  

### 非零的负整数  
	^-[1-9][]0-9"*$  
	^-[1-9]d*$  

### 非负整数  
	^d+$  
	^[1-9]d*|0$  

### 非正整数  
	^-[1-9]d*|0$  
	^((-d+)|(0+))$  

### 非负浮点数  
	^d+(.d+)?$  
	^[1-9]d*.d*|0.d*[1-9]d*|0?.0+|0$  

### 非正浮点数  
	^((-d+(.d+)?)|(0+(.0+)?))$  
	^(-([1-9]d*.d*|0.d*[1-9]d*))|0?.0+|0$  

### 正浮点数  
	^[1-9]d*.d*|0.d*[1-9]d*$  
	^(([0-9]+.[0-9]*[1-9][0-9]*)|([0-9]*[1-9][0-9]*.[0-9]+)|([0-9]*[1-9][0-9]*))$  

### 负浮点数  
	^-([1-9]d*.d*|0.d*[1-9]d*)$  
	^(-(([0-9]+.[0-9]*[1-9][0-9]*)|([0-9]*[1-9][0-9]*.[0-9]+)|([0-9]*[1-9][0-9]*)))$  

### 浮点数  
	^(-?d+)(.d+)?$  
	^-?([1-9]d*.d*|0.d*[1-9]d*|0?.0+|0)$  

