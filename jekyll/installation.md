Installing Jekyll on Ubuntu 14.04
---


```
sudo apt-add-repository ppa:brightbox/ruby-ng
sudo apt-get update
```


```
$ sudo apt-get install ruby2.4 ruby2.4-dev
Reading package lists... Done
Building dependency tree       
Reading state information... Done
ruby2.4 is already the newest version.
The following NEW packages will be installed
  ruby2.4-dev
0 to upgrade, 1 to newly install, 0 to remove and 496 not to upgrade.
Need to get 1,064 kB of archives.
After this operation, 4,957 kB of additional disk space will be used.
Do you want to continue? [Y/n] Y

```


```
$ sudo gem install jekyll bundler
Building native extensions.  This could take a while...
Successfully installed ffi-1.9.18
Fetching: rb-inotify-0.9.10.gem (100%)
Successfully installed rb-inotify-0.9.10
Fetching: sass-listen-4.0.0.gem (100%)
Successfully installed sass-listen-4.0.0
Fetching: sass-3.5.1.gem (100%)
Successfully installed sass-3.5.1
Fetching: jekyll-sass-converter-1.5.0.gem (100%)
Successfully installed jekyll-sass-converter-1.5.0
Fetching: listen-3.0.8.gem (100%)
Successfully installed listen-3.0.8
Fetching: jekyll-watch-1.5.0.gem (100%)
Successfully installed jekyll-watch-1.5.0
Fetching: kramdown-1.14.0.gem (100%)
Successfully installed kramdown-1.14.0
Fetching: liquid-4.0.0.gem (100%)
Successfully installed liquid-4.0.0
Fetching: mercenary-0.3.6.gem (100%)
Successfully installed mercenary-0.3.6
Fetching: forwardable-extended-2.6.0.gem (100%)
Successfully installed forwardable-extended-2.6.0
Fetching: pathutil-0.14.0.gem (100%)
Successfully installed pathutil-0.14.0
Fetching: rouge-1.11.1.gem (100%)
Successfully installed rouge-1.11.1
Fetching: safe_yaml-1.0.4.gem (100%)
Successfully installed safe_yaml-1.0.4
Fetching: jekyll-3.5.1.gem (100%)
Successfully installed jekyll-3.5.1
Parsing documentation for ffi-1.9.18
Installing ri documentation for ffi-1.9.18
Parsing documentation for rb-inotify-0.9.10
Installing ri documentation for rb-inotify-0.9.10
Parsing documentation for sass-listen-4.0.0
Installing ri documentation for sass-listen-4.0.0
Parsing documentation for sass-3.5.1
Installing ri documentation for sass-3.5.1
Parsing documentation for jekyll-sass-converter-1.5.0
Installing ri documentation for jekyll-sass-converter-1.5.0
Parsing documentation for listen-3.0.8
Installing ri documentation for listen-3.0.8
Parsing documentation for jekyll-watch-1.5.0
Installing ri documentation for jekyll-watch-1.5.0
Parsing documentation for kramdown-1.14.0
Installing ri documentation for kramdown-1.14.0
Parsing documentation for liquid-4.0.0
Installing ri documentation for liquid-4.0.0
Parsing documentation for mercenary-0.3.6
Installing ri documentation for mercenary-0.3.6
Parsing documentation for forwardable-extended-2.6.0
Installing ri documentation for forwardable-extended-2.6.0
Parsing documentation for pathutil-0.14.0
Installing ri documentation for pathutil-0.14.0
Parsing documentation for rouge-1.11.1
Installing ri documentation for rouge-1.11.1
Parsing documentation for safe_yaml-1.0.4
Installing ri documentation for safe_yaml-1.0.4
Parsing documentation for jekyll-3.5.1
Installing ri documentation for jekyll-3.5.1
Done installing documentation for ffi, rb-inotify, sass-listen, sass, jekyll-sass-converter, listen, jekyll-watch, kramdown, liquid, mercenary, forwardable-extended, pathutil, rouge, safe_yaml, jekyll after 38 seconds
Successfully installed bundler-1.15.3
Parsing documentation for bundler-1.15.3
Done installing documentation for bundler after 8 seconds
16 gems installed

```



# Opening the Firewall


```
$ sudo ufw allow 4000
Rule added
Rule added (v6)
```


```
$ sudo ufw status
Status: active

To                         Action      From
--                         ------      ----
Anywhere on eth0           ALLOW       169.254.0.0/16
4000                       ALLOW       Anywhere
4000 (v6)                  ALLOW       Anywhere (v6)
```



# References

* https://www.digitalocean.com/community/tutorials/how-to-set-up-a-jekyll-development-site-on-ubuntu-16-04
* for ruby2.4-dev:  https://gist.github.com/johngerome/133b127c9f8545dccc54


