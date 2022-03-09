# All you need to know to survive Vim

It's happened to us all. There you are, successfully navigating the black box of doom, a.k.a. The Terminal, showing off those nifty "mkdir" and "ls" skills, when BOOM! All of sudden you're in an alien world, where none of your keyboard presses work as expected...HEEEEELLLLPPP!


![Welcome to Vimland](https://cdn.hashnode.com/res/hashnode/image/upload/v1617717682799/7dxs5ue0u.png)

This is the world of Vim. 

For those of you that don't know, Vim is a command line text editor that comes free and pre-installed with many Linux distributions. If you've entered Vim accidentally, it's probably because you're being asked to change some code settings, and Vim has been assigned the default editor for this task. 

### Vim is weird

Vim doesn't work like many other editors. In fact, the first thing you'll notice is that it is completely mouse-less. Using the mouse won't work at all, so you need to know some specific keyboard commands to navigate and get out of Vimland. 

### Two common scenarios

We're going to go through how to deal with two very common scenarios:
1. How to just get out of Vim as fast as possible.
2. How to make a simple change to the file, then exit Vim safely. 

### Vim Modes

Firstly, it's very important to know that Vim has two modes:

- **Command mode**: this is the mode you are in when Vim first starts. You can't write any text when you are in this mode - most key presses map to some powerful Vim command instead.
- **Insert mode**: this is the mode you would need to be in to write to the file (insert any text). Keyboard presses work relatively normally in this mode. 

### Getting the hell out of Vim

You use "Esc" to enter command mode. My top advice for anyone that has flailed around Vim for a while unexpectedly is to STOP, press `ESC` and then press the following keys (exactly as written) to get out of vim: 

```
:q!
```

![there must be some meaning](https://media.giphy.com/media/WUx4Bp8yB0vIBzUqJb/giphy.gif)

This combination of `Esc` + `:q!` means **"Enter command mode, then force quit Vim, discarding all changes"**. 

The `q` is for "quit", the exclamation mark is for "force" and the fact that we haven't added a `w` (for "write") means we are not saving any changes to the file.  

If you just want to get the hell out of Vim, the above should work for you. If you accidentally press any keys wrong, just press ESC again and start typing the command again. 

### Making simple file changes

Remember, when you first enter Vim you will be in Command mode. To edit the file, you will need to enter Insert mode. 

To do this, you simply press `i`. 

You should see `--INSERT --` appear at the bottom of the screen. If this isn't working, deploy my top tip (press ESC) and try again. 

Now you should be able to move around the text with your arrow keys and add stuff as normal. 

Once you're done, you need to enter Command mode again (with ESC), and quit the editor, this time using "w" to "write" the changes to the file, i.e. to save it. 

`Esc` + `:wq`

### You survived! ![You survived!](https://media.giphy.com/media/3gM1liq7Eetk4/giphy.gif)

And that's it! If you hate Vim, these commands are all you'll ever need to know! 

![There's more!](https://media.giphy.com/media/26mfgndDD21nHtj2g/giphy.gif)

If it turns out that you don't hate Vim after all, then there are hundreds more commands that do lots of really cool things. 

You might turn into one of those coders that exclusively writes code in Vim. :O  

![Genius cat](https://media.giphy.com/media/xT77XZrTKOxycjaYvK/giphy.gif)

If that's you, see the [Linux handbook](https://linuxhandbook.com/basic-vim-commands/) for more basic commands. 
