# wubba-lubba-dub-dub
I am in great pain, please help me aka Rick and Morty quotes in the shell  

Inspired by [vsbuffalo's](https://github.com/vsbuffalo) [good-news-everyone](https://github.com/vsbuffalo/good-news-everyone). Some code borrowed.

Get Rick and Morty quotes in your shell! 

![screenshot](http://url/to/img.png)

## Installation
From the command line, run the following:
```
curl -s https://raw.githubusercontent.com/cjfiscus/wubba-lubba-dub-dub/master/rickandmorty.txt |\awk '{print $0} END{print "total quotes: "NR > "/dev/stderr"}' > ~/.rickandmorty.txt
```

Add the following line to your ```~/.bashrc```, ```~/.zshrc```, or ```~/. bash_profile```
```
# wubba-lubba-dub-dub
head -$((${RANDOM} % `wc -l < file` + 1)) ~/.rickandmorty | tail -1
```

 
