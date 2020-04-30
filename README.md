# constructorDiv
 Using the constructor, create a div with various parameters and add text to it.

First we create a class and call it “Option”, ***but you can name it whatever you want***.

**The name must begin with a capital letter!**

<code>class Options {}</code>

The second step is to give properties to our class:

**In our case, it will be:** ***height, width, bg, fontSize, textAlign***

That's what happened:

<code>constructor(height, width, bg, fontSize, textAlign)</code>

We declare methods:

<code>this.height = height;</code>

The next step is to add a method called "create", but you can name it whatever you like.

In parentheses indicate the argument "text" to our method.

<code>create(text) {}</code>

The method will create a new div:

<code>let div = document.createElement('div');</code>

Using "innerHTML" we will write any text in the div:

<code>div.innerHTML = `<h1>${text}</h1>`;</code>

and with the help of "cssText" we will change its style from the passed parameters:

<code>div.style.cssText = `height:${this.height}; width:${this.width}; background:${this.bg}; font-size:${this.fontSize}; text-align:${this.textAlign}`;</code>

Also, do not forget to add a div to our project. In our case, we add it directly to the body:

<code>document.body.appendChild(div);</code>

Next, we exit the local execution area of the create method and class.

Create a new object through class with arguments corresponding to "constructor":

<code>let block = new Options('40%', '30%', 'pink', '14px', 'center');</code>

We call the method of the new object, pass any text to the argument and get the element in our project:

<code>block.create('We did it all!');</code>
