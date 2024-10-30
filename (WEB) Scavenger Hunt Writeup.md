# Description: 

There is some interesting information hidden around this site http://mercury.picoctf.net:27278/. Can you find it?

# Solution:

The challenge gives us a link which opens a webpage with some standard HTML and nothing much more. Considering the name of the challenge we can deduce that this is a standard
inspect element challenge. Right-clicking the page and clicking 'Inspect Element' we begin to do some reconnaissance on the website. In the 'index.html' file under "Sources"
we see a comment that gives us the first part of the flag
```
<!-- Here's the first part of the flag: picoCTF{t -->
```

In the 'mycss.css' file also under "Sources" we see another comment that gives us the second part of the flag
```
/* CSS makes the page look nice, and yes, it also has part of the flag. Here's part 2: h4ts_4_l0 */
```

In the 'myjs.js' file under "Sources" we see yet another comment that hints us at the next part of the challenge
```
/* How can I keep Google from indexing my website? */
```

Using this hint we can deduce the next part of the flag will be in the robots.txt file of webpage which is a file that tells search-engine crawlers which pages can or can't be
requested. Heading to http://mercury.picoctf.net:27278/robots.txt we see:
```
User-agent: *
Disallow: /index.html
# Part 3: t_0f_pl4c
# I think this is an apache server... can you Access the next flag?
```

Using the apache server hint we try the '.htaccess' default apache file at http://mercury.picoctf.net:27278/.htaccess
```
# Part 4: 3s_2_lO0k
# I love making websites on my Mac, I can Store a lot of information there.
```

After doing some research about default Mac files relating to Store we find the ".DS_Store" file and get the last part of the flag from http://mercury.picoctf.net:27278/.DS_Store
```
Congrats! You completed the scavenger hunt. Part 5: _a69684fd}
```

This challenge really just required knowing how to view the source files of a page, having some knowledge of basic default web files, and doing some research based off the hints
that were given to us.