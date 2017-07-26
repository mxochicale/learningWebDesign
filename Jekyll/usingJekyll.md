

https://www.digitalocean.com/community/tutorials/how-to-set-up-a-jekyll-development-site-on-ubuntu-16-04


# Creating a New Development Site


cd ~ && jekyll new www

```
$ jekyll new www
Running bundle install in /home/map479-admin/www...


Your user account isn't allowed to install to the system RubyGems.
  You can cancel this installation and run:

      bundle install --path vendor/bundle

  to install the gems into ./vendor/bundle/, or you can enter your password
  and install the bundled gems to RubyGems using sudo.

  Password: /var/lib/gems/2.4.0/gems/jekyll-3.5.1/lib/jekyll/utils/exec.rb:16:in `read': Interrupt
	from /var/lib/gems/2.4.0/gems/jekyll-3.5.1/lib/jekyll/utils/exec.rb:16:in `run'
	from /var/lib/gems/2.4.0/gems/jekyll-3.5.1/lib/jekyll/commands/new.rb:140:in `block in bundle_install'
	from /var/lib/gems/2.4.0/gems/jekyll-3.5.1/lib/jekyll/commands/new.rb:139:in `chdir'
	from /var/lib/gems/2.4.0/gems/jekyll-3.5.1/lib/jekyll/commands/new.rb:139:in `bundle_install'
	from /var/lib/gems/2.4.0/gems/jekyll-3.5.1/lib/jekyll/commands/new.rb:129:in `after_install'
	from /var/lib/gems/2.4.0/gems/jekyll-3.5.1/lib/jekyll/commands/new.rb:38:in `process'
	from /var/lib/gems/2.4.0/gems/jekyll-3.5.1/lib/jekyll/commands/new.rb:17:in `block (2 levels) in init_with_program'
	from /var/lib/gems/2.4.0/gems/mercenary-0.3.6/lib/mercenary/command.rb:220:in `block in execute'
	from /var/lib/gems/2.4.0/gems/mercenary-0.3.6/lib/mercenary/command.rb:220:in `each'
	from /var/lib/gems/2.4.0/gems/mercenary-0.3.6/lib/mercenary/command.rb:220:in `execute'
	from /var/lib/gems/2.4.0/gems/mercenary-0.3.6/lib/mercenary/program.rb:42:in `go'
	from /var/lib/gems/2.4.0/gems/mercenary-0.3.6/lib/mercenary.rb:19:in `program'
	from /var/lib/gems/2.4.0/gems/jekyll-3.5.1/exe/jekyll:13:in `<top (required)>'
	from /usr/local/bin/jekyll:22:in `load'
	from /usr/local/bin/jekyll:22:in `<main>'


```


add export GEM_HOME=$HOME/.gem to your .bash_profile -- this solves sudo issue on Mac OS and other unix systems.
You then also might need to have access to gems that provide executables (such as bundler), so add this too:
PATH=$PATH:$HOME/.gem/bin




```
jekyll new www
Running bundle install in /home/map479-admin/www...
  Bundler: The dependency tzinfo-data (>= 0) will be unused by any of the platforms Bundler is installing for. Bundler is installing for ruby but the dependency is only for x86-mingw32, x86-mswin32, x64-mingw32, java. To add those platforms to the bundle, run `bundle lock --add-platform x86-mingw32 x86-mswin32 x64-mingw32 java`.
  Bundler: Fetching gem metadata from https://rubygems.org/...........
  Bundler: Fetching version metadata from https://rubygems.org/..
  Bundler: Fetching dependency metadata from https://rubygems.org/.
  Bundler: Resolving dependencies...
  Bundler: Using public_suffix 2.0.5
  Bundler: Using bundler 1.15.3
  Bundler: Using colorator 1.1.0
  Bundler: Using ffi 1.9.18
  Bundler: Using forwardable-extended 2.6.0
  Bundler: Using rb-fsevent 0.10.2
  Bundler: Using kramdown 1.14.0
  Bundler: Using liquid 4.0.0
  Bundler: Using mercenary 0.3.6
  Bundler: Using rouge 1.11.1
  Bundler: Using safe_yaml 1.0.4
  Bundler: Using addressable 2.5.1
  Bundler: Using rb-inotify 0.9.10
  Bundler: Using pathutil 0.14.0
  Bundler: Using sass-listen 4.0.0
  Bundler: Using listen 3.0.8
  Bundler: Using sass 3.5.1
  Bundler: Using jekyll-watch 1.5.0
  Bundler: Using jekyll-sass-converter 1.5.0
  Bundler: Using jekyll 3.5.1
  Bundler: Fetching jekyll-feed 0.9.2
  Bundler: Installing jekyll-feed 0.9.2
  Bundler: Fetching minima 2.1.1
  Bundler: Installing minima 2.1.1
  Bundler: Bundle complete! 4 Gemfile dependencies, 22 gems now installed.
  Bundler: Use `bundle info [gemname]` to see where a bundled gem is installed.
New jekyll site installed in /home/map479-admin/www.

```


```
$ bundle install
Using public_suffix 2.0.5
Using bundler 1.15.3
Using colorator 1.1.0
Using ffi 1.9.18
Using forwardable-extended 2.6.0
Using rb-fsevent 0.10.2
Using kramdown 1.14.0
Using liquid 4.0.0
Using mercenary 0.3.6
Using rouge 1.11.1
Using safe_yaml 1.0.4
Using addressable 2.5.1
Using rb-inotify 0.9.10
Using pathutil 0.14.0
Using sass-listen 4.0.0
Using listen 3.0.8
Using sass 3.5.1
Using jekyll-watch 1.5.0
Using jekyll-sass-converter 1.5.0
Using jekyll 3.5.1
Using jekyll-feed 0.9.2
Using minima 2.1.1
Bundle complete! 4 Gemfile dependencies, 22 gems now installed.
Use `bundle info [gemname]` to see where a bundled gem is installed.
map479-admin@EEE-003124:~/www$

```


```
vim _config.yml
```

```
#url: "http://example.com" # the base hostname & protocol for your site
```
:x



#  Starting Jekyll's Web Server
```
cd ~/www

```

```
$ jekyll serve --host=0.0.0.0
Configuration file: /home/map479-admin/www/_config.yml
            Source: /home/map479-admin/www
       Destination: /home/map479-admin/www/_site
 Incremental build: disabled. Enable with --incremental
      Generating...
                    done in 0.618 seconds.
 Auto-regeneration: enabled for '/home/map479-admin/www'
    Server address: http://0.0.0.0:4000/
  Server running... press ctrl-c to stop.


```

Open http://0.0.0.0:4000/ on firefox 
