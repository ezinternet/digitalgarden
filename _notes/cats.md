---
{"dg-publish":true,"permalink":"/0/070-book/library/","tags":"gardenEntry"}
---

# λμ 

## π¦ μ½κ³  μλ μ± 


```dataview
TABLE without id 
	status as "μν",
	("![coverimg|50](" + cover_url+ ")") as "λΆμ»€λ²",
	file.link as "λμλͺ", 
	category as "μΉ΄νκ³ λ¦¬", 
	dateformat(start_read_date, "DD") as "μμμΌ", 
	dateformat(finish_read_date, "DD") as "μλ£μΌ",
	my_rate as "λ΄ νμ ",
	book_note as "λ΄ μν"
FROM  #πλμ
       WHERE status = "π¦ μ§νμ€" and !contains(file.path, "Templates") 
       sort start_read_date desc 
```



## π§ μ½μ μ± 

```dataview 
TABLE without id
		status as "μν", 
		("![coverimg|50](" + cover_url+ ")") as "λΆμ»€λ²",
		file.link as "λμλͺ",
		category as "μΉ΄νκ³ λ¦¬", 
		 dateformat(start_read_date, "DD") as "μμμΌ",
		dateformat(finish_read_date, "DD") as "μλ£μΌ", 
		my_rate as "λ΄ νμ ",
		book_note as "λ΄ μν"
FROM #πλμ
          WHERE status = "π§ μμ " and !contains(file.path, "Templates")  
          SORT start_read_date desc 
``` 


## π¨ μ½λ€κ° λ―Έλ£¬ μ± 
```dataview 
TABLE without id 
	status as "μν", 
	("![coverimg|50](" + cover_url+ ")") as "λΆμ»€λ²",
	file.link as "λμλͺ", 
	category as "μΉ΄νκ³ λ¦¬",
	
	dateformat(start_read_date, "DD") as "μμμΌ", 
	dateformat(finish_read_date, "DD") as "μλ£μΌ", 
	my_rate as "λ΄ νμ ",
	book_note as "λ΄ μν"
FROM #πλμ  
	WHERE status = "π¨ μ°κΈ°" and !contains(file.path, "Templates")  
	SORT start_read_date desc
``` 


## π© λ€ μ½μ μ±
```dataview 
TABLE without id 
	status as "μν", 
	("![coverimg|50](" + cover_url+ ")") as "λΆμ»€λ²",
	file.link as "λμλͺ", 
	category as "μΉ΄νκ³ λ¦¬",
	
	dateformat(start_read_date, "DD") as "μμμΌ", 
	dateformat(finish_read_date, "DD") as "μλ£μΌ", 
	my_rate as "λ΄ νμ ",
	book_note as "λ΄ μν"
FROM #πλμ  
	WHERE status = "π© μλ£" and !contains(file.path, "Templates")  
	SORT start_read_date desc
``` 




------------------------
  -----------------------
--------------------  


```dataview
 Table description
 from [[#this.file.name]] and
 !outgoing([[#this.file.name]])

```

--------------------
--------------------

μΆμ²: [https://olait.tistory.com/31](https://olait.tistory.com/31) [Second Brain with Obsidian]


```
cssClasses : row-alt,table-small,col-lines,row-lines,table-numbers
```

#πλμ  #λμ  #library
