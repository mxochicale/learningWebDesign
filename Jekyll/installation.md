


# Installing Jekyll on Ubuntu 14.04

https://www.digitalocean.com/community/tutorials/how-to-set-up-a-jekyll-development-site-on-ubuntu-16-04

```
sudo apt-get update
```


```
$ sudo apt-get install ruby ruby-dev make gcc
Reading package lists... Done
Building dependency tree       
Reading state information... Done
gcc is already the newest version.
make is already the newest version.
make set to manually installed.
The following extra packages will be installed:
  libruby1.9.1 ruby1.9.1 ruby1.9.1-dev
Suggested packages:
  ri ruby1.9.1-examples ri1.9.1 ruby-switch
The following NEW packages will be installed
  libruby1.9.1 ruby ruby-dev ruby1.9.1 ruby1.9.1-dev
0 to upgrade, 5 to newly install, 0 to remove and 495 not to upgrade.
Need to get 3,567 kB of archives.
After this operation, 16.9 MB of additional disk space will be used.
Do you want to continue? [Y/n]


```

```
$ sudo gem install jekyll bundler
Fetching: public_suffix-2.0.5.gem (100%)
ERROR:  Error installing jekyll:
	public_suffix requires Ruby version >= 2.0.
Fetching: bundler-1.15.3.gem (100%)
Successfully installed bundler-1.15.3
1 gem installed
Installing ri documentation for bundler-1.15.3...
Installing RDoc documentation for bundler-1.15.3...
map479-admin@EEE-003124:~$

```

solving Ruby version >= 2.0. dependency:

sudo apt-get purge  ruby ruby-dev
```
$ sudo apt-get install ruby2.0 ruby2.0-dev
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following extra packages will be installed:
  libruby1.9.1 libruby2.0 ruby ruby1.9.1 rubygems-integration
Suggested packages:
  ri ruby-dev ruby1.9.1-examples ri1.9.1 ruby1.9.1-dev ruby-switch bundler
The following NEW packages will be installed
  libruby1.9.1 libruby2.0 ruby ruby1.9.1 ruby2.0 ruby2.0-dev
  rubygems-integration
0 to upgrade, 7 to newly install, 0 to remove and 495 not to upgrade.
Need to get 3,784 kB/6,475 kB of archives.
After this operation, 30.7 MB of additional disk space will be used.
Do you want to continue? [Y/n]
```


sudo apt-get purge  ruby ruby-dev


sudo apt-add-repository ppa:brightbox/ruby-ng
sudo apt-get update


```
$ sudo apt-get install ruby2.4
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following extra packages will be installed:
  libruby2.4 rubygems-integration
Suggested packages:
  bundler
The following NEW packages will be installed
  libruby2.4 ruby2.4 rubygems-integration
0 to upgrade, 3 to newly install, 0 to remove and 496 not to upgrade.
Need to get 3,746 kB of archives.
After this operation, 16.3 MB of additional disk space will be used.
Do you want to continue? [Y/n] Y

```


```
$ sudo gem install jekyll bundler
Fetching: public_suffix-2.0.5.gem (100%)
Successfully installed public_suffix-2.0.5
Fetching: addressable-2.5.1.gem (100%)
Successfully installed addressable-2.5.1
Fetching: colorator-1.1.0.gem (100%)
Successfully installed colorator-1.1.0
Fetching: rb-fsevent-0.10.2.gem (100%)
Successfully installed rb-fsevent-0.10.2
Fetching: ffi-1.9.18.gem (100%)
Building native extensions.  This could take a while...
ERROR:  Error installing jekyll:
	ERROR: Failed to build gem native extension.

    current directory: /var/lib/gems/2.4.0/gems/ffi-1.9.18/ext/ffi_c
/usr/bin/ruby2.4 -r ./siteconf20170727-6733-1y69u4j.rb extconf.rb
mkmf.rb can't find header files for ruby at /usr/lib/ruby/include/ruby.h

extconf failed, exit code 1

Gem files will remain installed in /var/lib/gems/2.4.0/gems/ffi-1.9.18 for inspection.
Results logged to /var/lib/gems/2.4.0/extensions/x86_64-linux/2.4.0/ffi-1.9.18/gem_make.out
Fetching: bundler-1.15.3.gem (100%)
Successfully installed bundler-1.15.3
Parsing documentation for bundler-1.15.3
Installing ri documentation for bundler-1.15.3
Done installing documentation for bundler after 9 seconds
1 gem installed

```
https://gist.github.com/johngerome/133b127c9f8545dccc54


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
