
# Encyclopedia  `<dd>`

*The `<dd>` is a HTML tag belongs to HTML description lists and is used to describe a term/name in a description list.*


The `<dd>` tag is used in conjunction with `<dl>` and `<dt>` to build a description list.The `<dd>` tag can occur only as a child element of a description list and it must follow a `<dt>` or a `<dd>` element, inside a `<dl>`.The `<dl>` tag defines the description list, the `<dt>` tag contains the term (name) to be defined, and the `<dd>` tag contains the definition description content for each term. 

Inside a `<dd>` tag you can put paragraphs, line breaks, images, links, lists, etc. It represents the description, definition, or value, part of a term-description group in a description list.

The `<dd>` tag also supports the Global Attributes in HTML, which give elements meaning and context. Also, it supports the Event Attributes in HTML.


## Syntax

`<dd>` is a HTML tag and must have a start tag. The end tag may be omitted if this element is immediately followed by another `<dd>` element, or if there is no more content in the parent element.


```
        <dl>
        	<dt>Item Name</dt>
        		<dd>Description for Item</dd>
        </dl>
```



## Example 1

Here are two simple examples showing the difference between a description list and an unordered list.

```
<ul>
  <li>Coffee</li>
  <li>Tea
    <ul>
      <li>Black tea</li>
      <li>Green tea</li>
    </ul>
  </li>
  <li>Milk</li>
</ul>

```

```
  <dl>
	  <dt>Coffee</dt>
	  <dd>Black hot drink</dd>
	  <dd>White cold drink</dd>
	  <dt>Tea</dt>
	  <dd>Black tea</dd>
	  <dd>Green tea</dd>
	  <dt>Milk</dt>
	</dl>

```

## Example 2

A FAQ sample by using structure of a description list.

```
	<article>
		 <h1>FAQ</h1>
		 <dl>
		  <dt>What do we want?</dt>
		  <dd>Our data.</dd>
		  <dt>When do we want it?</dt>
		  <dd>Now.</dd>
		  <dt>Where is it?</dt>
		  <dd>We are not sure.</dd>
		 </dl>
	</article>
		
```

## Example 3

Description lists are useful for displaying metadata as a list of key-value pairs.

```
	
	<dl>
	    <dt>Name</dt>    
	    <dd>Godzilla</dd>
	    <dt>Born</dt>
	    <dd>1952</dd>
	    <dt>Birthplace</dt>
	    <dd>Japan</dd>
	    <dt>Color</dt>
	    <dd>Green</dd>
	</dl>

```

## Example 4 - Complex

Together with `<dl>`, `<dd>` can be used to define a vocabulary list, like in a dictionary. In the following example, each entry, given by a `<dt>` with a `<dfn>`, has several `<dd>`s, showing the various parts of the definition.


```
    <dl>
		 <dt><dfn>happiness</dfn></dt>
		 <dd class="pronunciation">/'hæ p. nes/</dd>
		 <dd class="part-of-speech"><i><abbr>n.</abbr></i></dd>
		 <dd>The state of being happy.</dd>
		 <dd>Good fortune; success. <q>Oh <b>happiness</b>! It worked!</q></dd>
		 <dt><dfn>rejoice</dfn></dt>
		 <dd class="pronunciation">/ri jois'/</dd>
		 <dd><i class="part-of-speech"><abbr>v.intr.</abbr></i> To be delighted oneself.</dd>
		 <dd><i class="part-of-speech"><abbr>v.tr.</abbr></i> To cause one to be delighted.</dd>
	</dl>
```

## Special Notes


The `<dd>` tag is different from `<dt>` tag because the content of `<dd>` tag can be formatted further using headings (`h1`, `h2`, etc.), paragraphs (`p`) and blockquotes, as well as Inline and Phrase Elements.

A significant tip for using `<dd>` tag is that do not use this element (nor `<ul>` elements) to merely create indention on a page. Although it works, this is a bad practice and obscures the meaning of definition lists.

To change the indention of a description term, use the CSS margin property.



## Browser compatibility:

Chrome, Internet Explorer, Firefox(Gecko), Safari, Opera 
all support this element.



## References

1. [W3School](http://www.w3schools.com/TAgs/tag_dd.asp)
2. [MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/dl#examples)
3. [HTML Standard Document](https://html.spec.whatwg.org/multipage/semantics.html#the-dd-element)


# Encyclopedia  `margin-left`

*`margin-left` defines the horizontal distance from the left border edge of the element.*

The CSS `margin` properties are used to generate space around elements. The `margin-left` property set the left size of the white space outside the border. 


## Syntax

The `margin-left` has four values to take:

```
        margin-left: <length | percentage | auto | inherit>;
```

### Values

As one of individual margin properties, `margin-left` have four values as following:
	
* auto - the browser calculates the margin
* length - specifies a margin in px, pt, cm, etc.
* % - specifies a margin in % of the width of the containing element
* inherit - specifies that the margin should be inherited from the parent element

Tip: Negative values are allowed.

Note that even for the top and bottom margins the percentage value will refer to the width of the containing block.

#### length

It specifies a fixed width: it can be absolute width, e.g. in px(pixels),pt(points), or a width relative to the text size, e.g. in em, or relative to the viewport size, e.g. in vh.

```

p {
	margin-left: 2cm;
}

```

In example above, the `p` element is pushed over to the right `2cm` by seeting `margin-left` of 2 centimeters.

#### percentage

A percentage of the width of the containing block. Negative values are allowed. 

```

p {
	margin-left: -10%;
}

```
The `p` element has a `margin-left` of `-10%` set on it, meaning that it is pushed over to the left by 10% of the parent element's width. 

#### auto

You can set the `margin-left` as `auto` indicating that the left margin receives a share of the remaining space, defined mainly by the current layout mode.

#### inherit

If `margin-left` takes `inherit` as its values, it means that the left margin will be inherited from the parent element:

```

div.container {
    border: 1px solid red;
    margin-left: 100px;
}

p.one {
    margin-left: inherit;
}

```

In this example, `div.container` is parent of `p.one` so `p.one` gets `margin-left: 100px` by setting value `inherit`.


## Example 1

The following example sets absolute length of `80px` for left margin of a `<p>` element:

```
        p {
        	margin-left: 80px;
        }
```

## Example 2

The following example has a length relative to the text size.


```
        p {
        	margin-left: 1em;   
        }
```

## Example 3 - Complex

When you apply percentage to left margin of an element, the browsers will calculate actual size of the left margin by multiplying the percentage against the `width` of the parent node.

```
   <div style="width: 20px">
	<div id="child" style="margin-left: 25%">Test left</div>
	</div> 
```

Then you will have the following result:

	child.marginLeft = 20px * 25% = 5px;

When you try to apply `margin-left` to any non-statically positioned element, it relative to the `height` element of parent node instead of the `width`. For example:

```

<div style="height: 100px; width: 50px">
<div id="child" style="position: relative; left: 25%">Test left</div>
</div>

```

In this case, you will have the following result:

	child.marginLeft = 100px * 25% = 25px;


## Special Notes

If the element to the side is floated, or absolutely positioned, the margin will pass through it, because floats and absolute elements are removed from the flow. The margin will only be affected by static elements (or elements for which position is set to relative, and which have no coordinates) in the normal flow of the document—this includes the containing block itself.


## Browser compatibility:

Chrome 1.0, Internet Explorer 6.0, Firefox(Gecko) 1.0, Safari 1.0,Opera 3.5 all support `margin-left` property.


## References

1. [W3School](http://www.w3schools.com/TAgs/tag_dd.asp)
2. [MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/dl#examples)
3. [sitepoint](http://reference.sitepoint.com/css/margin-left)
 


# Encyclopedia `String.prototype.slice()`

*The JavaScript string method `String.prototype.slice()` extracts a portion of a string and returns a new string.*


## Syntax

The string function `.slice()` have one required parameter `beginSliceIndex` and one optional parameter `endSliceIndex`.

```
        str.slice(beginSliceIndex[, endSliceIndex]);
```

#### beginSliceIndex

The zero-based index where the slice should begin. If `beginSliceIndex` is a negative number, it is treated as `sringLength + beginSliceIndex `. For example, if beginSliceIndex is `-3` it is treated as `stringLength - 3`.

#### endSliceIndex

Optional. The zero-based index where the slice should end. If it is omitted, the substring will consist of the start index all the way through the end of the string. For method `.slice()` this parameter is exclusive; that is, the resultant substring will not contain the character at the final index. Similar to `beginSliceIndex` parameter, if it is negative, it is treated as `sringLength + endSliceIndex `.

## Example 1

Here is a simple example to test two parameters of `.slice()` method:

```
        var str = "hello world!";
        console.log(str.slice(0));	//-> "hello world!"
        console.log(str.slice(0, 5)); //-> "hello"
        console.log(str.indexOf("o")); //-> 4
```

In example above, if we start from beginning and ommit the `endSliceIndex`, we will get the whole string. If we set the start point and end point to `0` and `5`, we will get the substring `hello`. Let's check whether the `endSliceIndex` is exclusive by calculating the index of last element `o` in substring `hello`, the result is `4`, which is different from value of our `endSliceIndex`.

## Example 2

If the index is out of range, it returns the empty string.

```
	var str = "hello world!";
	console.log(str.length);		//-> 12
	console.log(str.slice(20, 1));	//-> ""

```


## Example 3 - Complex

The example below is to illustrate effects of the negtive number to parameters of `.slice()` method: 

```
        var str = "hello world!";
        console.log(str.length);		//-> 12
        console.log(str.slice(-6));	//-> "world!"
        console.log(str.indexOf("w")); //-> 6 = 12 -6
        console.log(str.slice(-6, -1)); //-> "world"
        console.log(str.indexOf("d")); //-> 10 = (12-6, 12-1)
        console.log(str.slice(2, -1)); //-> "llo world"
        console.log(str.indexOf("l")); //-> 2 = (2, 12-1)
```

In this example, the length of string is 12, we set `-6` to `beginSliceIndex` parameter and we get a substring "world!" which exactly start from index `6`. We set `-1` to the `endSliceIndex` and we get a substring ends with index `10`.

## Special Notes

There are some functions in JavaScript about string have similar usage such as `String.prototype.substr()` and ` String.prototype.substring()`. Sometimes you will be confused about making a choice. So whenever you are in doubt which function should be used, think about your parameter and read the description of the functions. 

## References

1. [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/slice)
2. [blog](https://blog.tompawlak.org/javascript-slice-substr-substring)