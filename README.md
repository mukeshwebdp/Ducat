### HTML (Hyper Text Markup Language)
***
**Website:** Collection of webpage is called website.

**Static:** A static website is a website made up fixed code and pre-built files

**Dynamic:** Dynamic website is a website containing data that can be mutable and changeable.


>**Note:**
>
>* Frontent ka code user ke Browser par execute hota hai.
>
>* Backend server par execute hota hai.




**HMTL:** Fist launch `1989` testing phase, Final launch `1991` and latest update `2014` HTML5.

**Tag:** its called tag `<>`

**There are three types of tags:** 

1. **Empty Tag:** Only opening bracket not clossing.
2. **Container Tag:** Opening and clossing bracket `<></>`
3. Comment Tag: `<!--   data  -->`

**`<sub>` Tag:** used to display text as a subscript.
**Example:** 

```HTML
<p>H<sub>2</sub>O<p>
```

**`<sup>` Tag:** used to display text as a subscript.

```HTML
<p>6<sup>2</sup>O<p>
```

**`<pre>`:** Tag define prefromatted text, which is displayed in a fixed-width font and preserves spaces and line bracks. this tag is useful for displaying text where typographical formatting offects the meaning of the context.**(jaisa content type karoge waisa content output milega "pre tag hamesha multiple line me kam karta hai single line me nahi")**

```HTML
<pre>Hello 
            world
    with Mukesh.
</pre>
```

**Some tags are usecase:** 

1. `<b></b>`: text Bold.
2.  `<u></u>`: underline.
3.  `<i></i>`: Italic

***
## 13-06-2024

**Attributes:** Additional properties that can be add to HTML Elements to modifiy their behavior or display.

```HTML
<font color="red" size="-2 to +4" face="font-name"></font>

<p align="right,left,center"> only anyone use at a time </p> 
```

>**Note:**
>
> * `<center>` tag multiple tags ko center karne me use hota hai.
> * `align` attribute keval usi tag ko effect karega gis tag me assign ho.

**`<hr>` Attributes:**
```HTML 
    <hr color="red" size="8px" align="left,right,center">
    
 ```
 >**Note:**
 > 
 > * Web desining ki default unit pixel hoti hai hai pixel kabhi kishi par depend nahi rahata hai.
 > 
 >      1px = 1/96 * 1(inch)
 >
 >     1px = 1/96 * 2.54(cm)
 >* **Percentage(%):** Apane parent par depend rahata hai.
 >* **Multiple space:** -space ke liye `&nbsp;` isaka use karte hai.
 
 ```HTML
    <p> &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Hello</p>
 ```

### 19-06-2024

**`<marquee>`Tag:** content ko left, right, up, down  move karta hai.

Example: ⬅️, ➡️, ⬆️, ⬇️

**`<marquee>`Tag of attributs:** 

**bahavior:** The text within the marquee can scroll in three ways.
1. **scroll:** The text moves continuously.
2. **slide:** The text enters from one side.
3. **alternate:** The text move back and forth.
```HTML
   <marquee behavior="scroll,slide,alternate"> choose anyone </marquee>
```
**scrollamount:** 1 minutes me data kitani bar move karega usko define karta hai.

**height,width,bgcolor:** ye bhi `<marquee>` ke attribue hai, bgcolor- background color apply karne ke liye use hota hai.

```HTML
   <marquee height='10px' width='40%' bgcolor='red' scrollamount='20' > choose anyone </marquee>
```
**onmouseout:** ye ek JavaScript ka event hai jiska  use mouse ka pointer hatane par <ins> Active</ins> ho jata hai eska method <ins>start()</ins> jo by default hota hai, jiska use kisi bhi event ko start karne ke liye kiya jata hai.

**onmouseover:** ye bhi JavaScript ka event hai jiska use kisi bhi content ke upar mouse ka pointer point karte hai to yah <ins>Active</ins> ho jata hai eska method <ins>stop()</ins> kisi event ko rokane me use kiya jata hai.

**loop:** eska use katani bar attrition perform karni hai.

```HTML
   <marquee height='10px' width='40%' bgcolor='red' scrollamount='20' onmouseover='stop()' onmouseout='stop()' loop='10'> choose anyone </marquee>
```