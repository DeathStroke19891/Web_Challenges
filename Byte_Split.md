# Byte split

## Analysis

Probably my easiest challenge which is pretty straight forward. 
+ Download the exposed .git folder.
+ Recreate the worktree
+ Go into the extensions folder
+ View the background.js file, which has some chinese charecters

`浸穹㍷洶穪牤㝤㔷睰昷穬慧㝧楱栲㙱獢歴㔳㑺㑭㌳獵㕮潺瑲橶祤\u2e6f湩潮`

Now inspecting the binary data of a chinese character given, one can see that it is composed of 2 bytes each.
Spliting each character in the middle as the title suggests, gives an .onion link

`mxzy3wm6zjrd7d57wpf7zlag7giqh26qsbkt534z4m33su5noztrjvyd.onion`

Going to this tor website gives you the flag.

The worktree can be recreated from the objects using a tool like gittools or by learning about git internals from the link given below.

## Resources

[Link 1](https://medium.com/swlh/hacking-git-directories-e0e60fa79a36)

