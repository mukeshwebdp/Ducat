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

***\
### 20-06-2024

**Nested Marquee:** ek marquee ke andar dusra marquee hota hai use nested marquee kahate hai.
```HTML
<marquee behavior="alternate" width="80%"> 
   <marquee behavior="alternate" height=="20px" direction='down'>
      Hello world!
   </marquee>
</marquee>
```
**`<img>` tag:** `<img>` tag ka use web browser par image print karne ke liye kiya jata hai. ye ek empty tag hai.

```HTML
<img src='./path/file-name' >
```
**`<img>`<ins>Tag of attributes:**</ins>

**src:** src ka use path define karne ke liye hota hai.

**title:** title ka use image ko hover karne par message show karne ke liye hota hai.

```HTML
<img src="" title="hello world">
```
**target:** target ke two properties hote hai.

* 'self': self same page another web page ko load kar deta hai.
* _blank: _blank dusre tab par web page load karata hai.
```HTML
   <img src="" target="self"> // default.
   <img src="" target= "_blank"> // load another tap.
```

**`./`:** ye own directory ko represent karta hai.

**`../`:** ye parent directory ko represent karta hai. for example <ins>./demo/new-folder</ins>

### 21-06-2024
**List:**
There are three types of list:
* <ins>order list</ins>:  esme list ko aap count kar sakte hai, type: number, roman , alphabets. 
* <ins>unorder List:</ins> es kist me numbering nahi hota hai, eske type: circle, square, disc.
* <ins>Description List:</ins> The `<dl>` HTML element is used to create a description list. this list contains groups of terms and description the term are marked with `<dt>` elements and the description are marked with `<dd>` elements. Its often used for glossaries or lists of key-value pairs


**Order list of attributes:**

`type:` A,a,I,i

* A--> A,B,C,D
* a--> a,b,c,d,i
* I--> I, II, III, IV
* i--> i, ii, iii, iv

`reversed:` list ka numbering reverse karane ke liye kiya jata hai (eska effect listke item par nahi padata hai)
`start:` start attribute ka use apne echchha ke anusar number dene ke liye karte hai (eska use only number me kiya jata hai.)
```HTML
 <!-- A,B,C,B -->
<ol type='A'>
   <li>demo 1<li>
   <li>demo 2<li>
   <li>demo 3<li>
<ol>
<!-- a,b,c -->
<ol type='a'>
   <li>demo 1<li>
   <li>demo 2<li>
   <li>demo 3<li>
<ol>
   <!-- I, II, III -->
<ol type='I'>
   <li>demo 1<li>
   <li>demo 2<li>
   <li>demo 3<li>
<ol>
<!-- i, ii, iii -->
<ol type='i'>
   <li>demo 1<li>
   <li>demo 2<li>
   <li>demo 3<li>
<ol>
   <!-- Default : 1,2,3 -->
<ol >
   <li>demo 1<li>
   <li>demo 2<li>
   <li>demo 3<li>
<ol>
<!-- 3,2,1 -->
<ol resvered >
   <li>demo 1<li>
   <li>demo 2<li>
   <li>demo 3<li>
<ol>
   <!-- 40,41,42 -->
   <ol start="40" >
   <li>demo 1<li>
   <li>demo 2<li>
   <li>demo 3<li>
<ol>
```
**Unorder list of attributes:**
* `Type:`disc, circle, square
```HTML
<ul type="circle">
   <li>Demo 1</li>
   <li>Demo 2</li>
   <li>Demo 3</li>
</ul>
<ul type= 'disc'>
   <li>Demo 1</li>
   <li>Demo 2</li>
   <li>Demo 3</li>
</ul>
<ul type="square">
   <li>Demo 1</li>
   <li>Demo 2</li>
   <li>Demo 3</li>
</ul>
```

**Description list :**

```HTML
   <dl>
      <dt>HTML</dt>
      <dd> Lorem hello world!</dd>
   </dl>
```
**Nested list:** ek list ke under dusara list ho se nested list kahate hai.
```HTML
<ol>
   <li>Demo order list
      <ul>
         <li>Demo unorder list</li>
      </ul>
   </li>
</ol>
```
**Link or Hyperlink:**
* Local : agar aap own folder se <ins>href</ins> dete hai to use local link kahate hai.
* Global : different different website ka path add karne ho global link kahate hai.
* Internal Link : internal link ek hi page par lagta hai `<a href="#result">` id ka name bhi result dege.

```HTML
   <p id="result"> lorem  </p>
   
    
    <a href="#result">

```

`Anchor tag <a> :` It is used linking  to another webpage.
**Common Attributes:**
* `href`: URL of the page or resourse.
* `target`: where to open the link.
   * '_blank' : New tab/ window 
   * '_self' : same frame (default)

```HTML
<a href="www.google.com">Google</a>
<a href="www.google.com" target="_blank">Google</a>
<a href="www.google.com" target="_self">Google</a>

```
### 27-06
**favicon icon:** favicon icon ki size 15*15 or 20*20 honi chiye.
```HTML
<html>
   <head>
    <link rel="favicon icon" href="favicon.ico" type="image/x-icon">
      <tilte></titel>
      </head>
</html>
```
## Table:
collection of columns is called row, collection of rows is called table

`<th> or <thead> :` table heading.
`<td> :` table data.
`<tr> :` table row.
**Table of Attributs:**

`**cellspacing**`: cellspacing content ke out side work karti hai.
```HTML
      <table border="2px" cellspacing='10px'>
         <!-- effect content outside -->
         <tr>
            <th>Name</th>
            <th>Class</th>
            <th>Age</th>
         </tr>
         <tr>
               <td>Mukeh</td>
               <td>BCA</td>
               <td>21</td>
         </tr>
   </table>
```
`**cellspadding**`: cellspadding content ke inside work karti hai.
```HTML
      <table border="2px" cellspadding='10px'>
         <!--  content effect inside -->
         <tr>
            <th>Name</th>
            <th>Class</th>
            <th>Age</th>
         </tr>
         <tr>
               <td>Mukeh</td>
               <td>BCA</td>
               <td>21</td>
         </tr>
   </table>
```
`**rules:**` ke five properties hoti hai.
* all : table me single line ka border apply hoga
* rows: table me border only rows me apply hota hai.
* cols: table me border only columns me apply hota hai.
* none: columns aur rows ke border remove ho jayegi
* group: Default

```HTML
   <!-- table me single line ka border apply hoga -->
   <table border="2px" cellspadding='10px' rules="all">
         <tr>
            <th>Name</th>
            <th>Class</th>
            <th>Age</th>
         </tr>
         <tr>
               <td>Mukeh</td>
               <td>BCA</td>
               <td>21</td>
         </tr>
   </table>

   <!-- table me border only rows me apply hota hai. -->
   <table border="2px" cellspadding='10px' rules="rows">
         <tr>
            <th>Name</th>
            <th>Class</th>
            <th>Age</th>
         </tr>
         <tr>
               <td>Mukeh</td>
               <td>BCA</td>
               <td>21</td>
         </tr>
   </table>

<!-- table me border only columns me apply hota hai. -->
   <table border="2px" cellspadding='10px' rules="cols">
         <tr>
            <th>Name</th>
            <th>Class</th>
            <th>Age</th>
         </tr>
         <tr>
               <td>Mukeh</td>
               <td>BCA</td>
               <td>21</td>
         </tr>
   </table>

   <!-- table's all border none -->
   <table border="2px" cellspadding='10px' rules="none">
         <tr>
            <th>Name</th>
            <th>Class</th>
            <th>Age</th>
         </tr>
         <tr>
               <td>Mukeh</td>
               <td>BCA</td>
               <td>21</td>
         </tr>
   </table>
   <!-- default -->
   <table border="2px" cellspadding='10px' rules="group">
         <tr>
            <th>Name</th>
            <th>Class</th>
            <th>Age</th>
         </tr>
         <tr>
               <td>Mukeh</td>
               <td>BCA</td>
               <td>21</td>
         </tr>
   </table>

```

**colspan:** It is used to columns merge in the table.
**rowspan:** It is used to rows merge in the table.
```HTML
<table>
   <tr>
      <td colspan="3">User's</td>
      <td rowspan='3'>Teacher</td>
      <td>Name</td>
      <td>class</td>
      <td>Marks</td>
   </tr>
   <tr>
      <td colspan="3">User's</td>
      <td>Name</td>
      <td>class</td>
      <td>Marks</td>
   </tr>
</table>
```




