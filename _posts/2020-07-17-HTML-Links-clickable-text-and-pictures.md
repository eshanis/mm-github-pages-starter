---
published: true
Published: true
---
Sometimes you want to put links to others people's pages or pages within your own website.

For this, you use the "a" tags

**1. If you want to link to my github page**
```
<a href= "the_site_you_want_to_link"> The  Name of the site </a>
```

For example
```
 <a href="https://github.com/eshanis">  
    github Page      
 </a>
```

**2. Sometimes, you want to open the page in a new tab, so the user doesnt lose your page. Use "target=_blank"**
```
<a href= "the_site_you_want_to_link" target="_blank"> The  Name of the site you want to link to </a>
```

For example:
```
<!-- link to eshanis page WITH TARGET-->
<a href="https://github.com/eshanis"  target="_blank">      
	github Page       
</a>
```

**3. You may have noticed a title inside the opening "a" tag. This title shows up when you hover over the link**

For example:
```
  <!-- link to eshanis page WITH TITLE-->
<a href="https://github.com/eshanis"  target="_blank" title="star my github!">
</a>       
```


**4. In case you want to make an image as the thing you want the user to click to take them to another link**

For example
```
<a href="https://github.com/eshanis"  target="_blank" title="star my github!">
          <div>
            <img src="https://blog.eshani.ml/assets/images/eshu.jpg" alt="eshani" width="100" height="100">
          </div>      
</a>

```

**NOTE:** the use of "div" is optional.


**5. If you have many pages in your website and you want to link to another page in your website, you can do **
```
<a href="/html-tutorial1"  target="_blank" title="star my github!">
      
            <img src="https://blog.eshani.ml/assets/images/eshu.jpg" alt="eshani" width="100" height="100">
                
</a>
```
[tutorial 1](/html-tutorial1/)
So here's a complete example: 

