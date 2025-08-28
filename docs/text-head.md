# text Head
-----
`text;{params}`

-----
the text head does the obvious and displays text when placed down, this can be controlled via the paramaters

this will always be offset by default to be directly where the head is placed, but you can control this with the `pos` parameter

<b>if you provide a broken text or a broken property, the text may be stuck loading or the property will simply not load, as this is all type checked</b>

### IMPORTANT
this is like, the only head with different formatting and you have to append it in a different way compared to the normal paramater adding (<i>this is for better organization for me, but this can be changed in future if it's annoying for people</i>)

<b>you will need to format your data in the following way</b><br>
`{text=text, properties = {params}}`

i.e, a finalized text data with a gradient on it will look like the following:
<br>
`{text = "This is an example!", properties = {outline = true}`

<i>also make sure to stringify all vector 3's cuz userdata blah json blah</i>

-----
`Parameters - Base`
-----
-----
`text : String`
> The text that will be displayed on the text task of the head.

`properties : Table`
> The properties of the text task, all properties if valid will be applied to the TextTask. <i>(see paramaters below)</i>

---
`Paramaters - Properties`
----
----
`color : Hex / Vector3`
> Sets the color of the text. Will auto-convert Vector3 into Hex.

`pos : Vector3`
> Set the position of the text. This will default to 0,0,0 though first, and then will set the position afterwards.

`size : Number`
> Sets the size of the head via :setScale(), which will enlargen the TextTask

`outline : boolean`
> Sets the outline of the text to the boolean value.

`outline_color: Hex / Vector3`
> Sets the outline color of the text. Will auto-convert Vector3 into Hex

`align : "CENTER" | "LEFT" | "RIGHT"`
> Aligns the TextTask to the specificed values.

`gradient : table[Vector3, Vector3]`
> Sets the gradient of the text task from the 1st value to the 2nd value.

`shadow : boolean`
> Sets the shadow of the text to the boolean value.

`wrap : boolean`
> Sets the wrap of the text to the boolean value.

`opacity : number`
> Sets the opacity of the text task to the value.

`seeThrough : boolean`
> Makes the TextTask seethrough based on the value.

---
<center>[Go Back To Introduction](https://tivvo.github.io/astro-wiki/)</center>