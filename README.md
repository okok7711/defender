# Defender
---

> <picture>
>   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Mqxx/GitHub-Markdown/main/blockquotes/badge/light-theme/danger.svg">
>   <img alt="Danger" src="https://raw.githubusercontent.com/Mqxx/GitHub-Markdown/main/blockquotes/badge/dark-theme/danger.svg">
> </picture><br>
>
> **Warning Bad Code lies ahead**  
> **This code does not work on the latest version of fender i will need to rewrite practically all of it**  
> **In case you want to use it and don't care about being on the latest version, just `git reset --hard 0e7fa8425cc901bbe736c47dc84b3975dbcb60e0` in your `git clone`d Fender and then re-compile**

Some stuff written in [Fender](https://github.com/FenderLang/Fender/) for fun.
Feel free to open a PR and make it better or use my code for your projects!

### What this contains
Libraries:
- [Logic Gates](./libs/logic.fndr)
- [Bitwise Logic and other stuff](./libs/util.fndr)
- [Some Maths stuff](./libs/math.fndr)
- [Extended String Functionality](./libs/strings.fndr)
- [Extended Map Functionality](./libs/maps.fndr)
- [Extended Array Functionality](./libs/arrays.fndr)
- [JSON Parser](./libs/json.fndr)
- [Counter library](./libs/counter.fndr)
- [Type Library](./libs/types.fndr)
- [(small) Request Library](./libs/requests.fndr)

Other Stuff:
- [SHA-1](./sha.fndr)
- [Brainfuck](./brainfuck.fndr)
- [Arithmatic Logic Unit](./alu.fndr)
- [HTTPbin API Call](./httpbin.fndr)

### Why is this slow?
[Fender](https://github.com/FenderLang/Fender/) is still in a very early stage and therefore contains very few native functions which means that most of them have to be implemented using other basic functions in [Fender](https://github.com/FenderLang/Fender/).
The biggest bottleneck is probably the array clone function, as it has to iterate over all of the items of the array, instead of just making a clone in memory.
[Fender](https://github.com/FenderLang/Fender/) also has no documentation meaning that even if more efficient functions would exist I don't know of them :(

### *How* slow is this?
Well. The SHA-1 implementation took 840ms to hash `test`, while a poorly written and importless python implementation only took about 30ms.
When [Fender](https://github.com/FenderLang/Fender/) gets better this will be less of a problem due to more native functions being created and less functions having to be implemented by me who is not good at coding.

### If it's slow, why make it?
Dunno. It's fun to make stuff with something as barebones.
Speed is not really an issue for me and I enjoyed development of this project.

### What else to make
We'll see, maybe I'll implement some other algorithms in here or some entire libraries to do stuff? Maybe hashlib? Don't have any plans so I'm open for anything. If you want to have something made, open an issue and I'll try my best