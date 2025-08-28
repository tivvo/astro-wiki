
#  Introduction

  

if you're landing on this page, *i assume you* need some guidance around my current avatar and some of it's features, with this specifically being the head system right now
so hi! here's all the info that you actually need realistically


please note, all headers will be included at the top of each head class along with the paramaters after in code blocks

  

#  Quickstart - Formatting

`NOTE: all coup heads use this same formatting guide (json), and is done this way for ease of use when dealing with the actual heads, you can use toJson to just easily convert table with params`

  

##  Headers

all headers **control** whatever the head will do, you actually don't need a header at the start of the head to control it as the `;` (semi-colon) acts as a separator for the actual data of the head and the header itself

  

**this header does match 4p5's head format, with it being `header;{data}`**, so all you need to do is input a valid type for this header i.e `test;` or `test` for the head to be registered with the function of that header

  

**your skull data would look something like this if you want to register it with the test header:**

```md

SkullData: test;

*or*

SkullData: test

```

  

##  Data

data is controlled in a specific way, where you can easily pass a toJson and append it to the skull data with a table, **this must always be parsed after the seperator semi-colon `;`**

  

you can see the data available for every head in their pages specifically, and they will be listed like the following when available:

  

*example*

`kill : Boolean`

> Makes a confetti head explode other players within a 4 block vicinity, this does require the host of the head to be on however, as the kill command is ran by commands. Otherwise, it'll just summon the appear confetti effect on the players.

  

**this can be directly interpreted like most other tables in the following way:**

`{kill=true}`, with this you can then run a toJson call and encode it with base 64 after the header to the head, and it'll recognise that data afterwards

  

i.e

```lua
--- blah is a made up function for registering data heads with a header and then also data afterwards
blah.RegisterHead("confetti", toJson({kill=true}))
```

  

**no invalid param checking will be added, it'll just be ignored as it wont be used in the code (*except when said otherwise, but it's usually also ignored in that case too lmao*)**

  

----
### Heads
[Test Head](https://tivvo.github.io/astro-wiki/test-head)

[Text Head](https://tivvo.github.io/astro-wiki/text-head)

[Confetti Head](https://tivvo.github.io/astro-wiki/confetti-head)
