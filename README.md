# wubba-lubba-dub-dub
I am in great pain, please help me aka Rick and Morty quotes in the shell  

Inspired by [vsbuffalo's](https://github.com/vsbuffalo) [good-news-everyone](https://github.com/vsbuffalo/good-news-everyone). Installation code borrowed.

Get Rick and Morty quotes in your shell! 

![screenshot](http://url/to/img.png)

## Installation
From the command line, run the following:
```
curl -s https://raw.githubusercontent.com/cjfiscus/wubba-lubba-dub-dub/master/rickandmorty.txt |\awk '{print $0} END{print "total quotes: "NR > "/dev/stderr"}' > ~/.rickandmorty.txt
```

Add the following line to your ```~/.bashrc```, ```~/.zshrc```, or ```~/. bash_profile``` (MacoOS).
```
# wubba-lubba-dub-dub
head -$((${RANDOM} % `wc -l < ~/.rickandmorty.txt` + 1)) ~/.rickandmorty.txt | tail -1
```
Restart your terminal (or ```source ~/.bashrc``` or equivalent).

 
 
