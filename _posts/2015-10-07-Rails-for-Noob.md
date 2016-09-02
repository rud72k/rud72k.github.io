---
layout: post
title: "Rails for Noob (Part 1)"
description: "Installing ruby and rails in local machine"
location: "ruby world"
date: 2015-10-07
tags: 
- ruby
- update
- gems
- SSH
- rails
- SSL error
- sqlite3
---

# NOOB guides for Rails setup #

It's my first time learn rails. Sure I'm a noob in this area. What I did just roamed around looking for guide and stackexchange several time do this and that. Here's how do I do that. 

# First attempt #

As I use windows, I downloaded the ruby for windows in [rubyinstaller.org](rubyinstaller). As for the first timer, I just follow the basic: my laptop is 64bit so I need to download and install the 64bit version. 
<!--more-->

After workaround I thougt I was ready to learn rails. Then I typed

~~~
gem install rails
~~~

It worked. Then next time I tried was making the blog.

~~~
rails new blog
~~~

And I doomed. A lot of error showed up. What the...

~~~
/usr/local/lib/ruby/gems/2.0.0/gems/sqlite3-1.3.7/lib/sqlite3.rb:6:in `require': cannot load such file -- sqlite3/sqlite3_native (LoadError)
from /usr/local/lib/ruby/gems/2.0.0/gems/sqlite3-1.3.7/lib/sqlite3.rb:6:in `rescue in <top (required)>'
from /usr/local/lib/ruby/gems/2.0.0/gems/sqlite3-1.3.7/lib/sqlite3.rb:2:in `<top (required)>'
from /usr/local/lib/ruby/gems/2.0.0/gems/bundler-1.3.5/lib/bundler/runtime.rb:72:in `require'
from /usr/local/lib/ruby/gems/2.0.0/gems/bundler-1.3.5/lib/bundler/runtime.rb:72:in `block (2 levels) in require'
from /usr/local/lib/ruby/gems/2.0.0/gems/bundler-1.3.5/lib/bundler/runtime.rb:70:in `each'
from /usr/local/lib/ruby/gems/2.0.0/gems/bundler-1.3.5/lib/bundler/runtime.rb:70:in `block in require'
from /usr/local/lib/ruby/gems/2.0.0/gems/bundler-1.3.5/lib/bundler/runtime.rb:59:in `each'
from /usr/local/lib/ruby/gems/2.0.0/gems/bundler-1.3.5/lib/bundler/runtime.rb:59:in `require'
from /usr/local/lib/ruby/gems/2.0.0/gems/bundler-1.3.5/lib/bundler.rb:132:in `require'
from /home/manuele/Software/blog/config/application.rb:7:in `<top (required)>'
from /usr/local/lib/ruby/gems/2.0.0/gems/railties-4.0.0/lib/rails/commands.rb:76:in `require'
from /usr/local/lib/ruby/gems/2.0.0/gems/railties-4.0.0/lib/rails/commands.rb:76:in `block in <top (required)>'
from /usr/local/lib/ruby/gems/2.0.0/gems/railties-4.0.0/lib/rails/commands.rb:73:in `tap'
from /usr/local/lib/ruby/gems/2.0.0/gems/railties-4.0.0/lib/rails/commands.rb:73:in `<top (required)>'
from bin/rails:4:in `require'
from bin/rails:4:in `<main>'
~~~

Some said I had to install bundle. I did instal bundle by `gem install bundle' and it didn't work for me. Another Solution came from Vishnu in (stackoverflow)[vishnu]. He said:

> 
>
> Find your sqlite3 gemspec file. One example is /usr/local/share/gem/specifications/sqlite3-1.3.7.gemspec
>
> Windows: C:\Ruby21\lib\ruby\gems\2.1.0\specifications.
>
> You should adjust according with your Rubygem path and sqlite3 version. Edit the file above and look for the following line
>
> ~~~
> s.require_paths=["lib"]
> ~~~
> 
> change it to
>
> ~~~
> s.require_paths= ["lib/sqlite3_native"]
> ~~~
>

Some people have a good time but some people got sh\*t. I'm the second group. There's a looooot more error showed up. 

Then I uninstaled ruby gem from Control Panels on my Windows 10 and delete all the folder related to it.

# Second Attemp #

I started brand new start. I went to [rubyinstaller][rubyinstaller] again and read carefully. Then I found (maybe) the source of my problems. The 64bit-version is rather new. So maybe not all the gem, dependencies and anything, tested. Okay then. I'm just have to install 32bit version then. 

I installed ruby gems and its devkit without problems.

For safety, I installed bundle before install rails. I got no problem. 

I ran rails server

~~~
rails new blog
~~~

and it works. But it stopped at the middle of

~~~
...
run bundle

~~~

there's a gem dependency that I couldn't download. I was not suspiciousing anything. I try again after I install the gem 'he' wanted. But got another error with another gem. I think I had problem again here. 

Roamed around.

I got solution from roamed around in stackoverflow again. It says that it because SSL Error. The solution is in the gist [louislavena][ll] here : [link][ssl]. I copied it the new section

# SSL Solution #

## Installing using update packages (NEW)

Now that RubyGems 1.8.x, 2.0.x and 2.2.x have been released, you can manually
update to those versions.

First, download the proper version of RubyGems for your installation (eg.
if running version `1.8.28`, download `1.8.30`).

*Note*: To find the version of RubyGems you're using, please run `gem --version` in
the command line.

You can find download links at GitHub under
[Releases](https://github.com/rubygems/rubygems/releases).

Now, locate `rubygems-update-X.Y.Z.gem` where `X.Y.Z` will be the matching
version for the version of RubyGems you need to update:

- Running 1.8.x: download [1.8.30](https://github.com/rubygems/rubygems/releases/tag/v1.8.30)
- Running 2.0.x: donwload [2.0.15](https://github.com/rubygems/rubygems/releases/tag/v2.0.15)
- Running 2.2.x: download [2.2.3](https://github.com/rubygems/rubygems/releases/tag/v2.2.3)

Please download the file in a directory that you can later point to (eg. the
root of your harddrive `C:\`)

Now, using your Command Prompt:

```
C:\>gem install --local C:\rubygems-update-1.8.30.gem
C:\>update_rubygems --no-ri --no-rdoc
```

After this, `gem --version` should report the new update version.

You can now salefy uninstall `rubygems-update` gem:

```
C:\>gem uninstall rubygems-update -x
Removing update_rubygems
Successfully uninstalled rubygems-update-2.2.3
```

## Manual solution to SSL issue

If you have read the above detail that describe the issue, thank you.

Now, you want to manually fix the issue with your installation.

Steps are simple:

- Step 1: Obtain the new trust certificate
- Step 2: Locate RubyGems certificate directory in your installation
- Step 3: Copy new trust certificate
- Step 4: Profit

### Step 1: Obtain the new trust certificate

If you've read the previous sections, you will know what this means (and
shame on you if you have not).

We need to download [AddTrustExternalCARoot-2048.pem](https://raw.githubusercontent.com/rubygems/rubygems/master/lib/rubygems/ssl_certs/AddTrustExternalCARoot-2048.pem).

Use the above link and place/save this file somewhere you can later find
easily (eg. your Desktop).

**IMPORTANT**: File must have `.pem` as extension. Browsers like Chrome will
try to save it as plain text file. Ensure you change the filename to have
`.pem` in it after you have downloaded it.

### Step 2: Locate RubyGems certificate directory in your installation

In order for us copy this file, we need to know where to put it.

Depending on where you installed Ruby, the directory will be different.

Take for example the default installation of Ruby 2.1.5, placed in `C:\Ruby21`

Open a Command Prompt and type in:

```
C:\>gem which rubygems
C:/Ruby21/lib/ruby/2.1.0/rubygems.rb
```

Now, let's locate that directory. From within the same window, enter the path
part up to the file extension, but using backslashes instead:

```
C:\>start C:\Ruby21\lib\ruby\2.1.0\rubygems
```

This will open a Explorer window inside the directory we indicated.

### Step 3: Copy new trust certificate

Now, locate `ssl_certs` directory and copy the `.pem` file we obtained from
previous step inside.

It will be listed with other files like `GeoTrustGlobalCA.pem`.

### Step 4: Profit

There is actually no step 4. You should be able to install Ruby gems without
issues now.


# Now #

I run rails and server by typed

~~~
rails new blog2
cd bin
rails server
~~~

and it works. 

Lets learn a lot.



[rubyinstaller]: http://rubyinstaller.org
[vishnu]: http://stackoverflow.com/questions/17643897/cannot-load-such-file-sqlite3-sqlite3-native-loaderror-on-ruby-on-rails
[ll]: https://github.com/luislavena
[ssl]: http://help.rubygems.org/discussions/problems/19586/r?go=aHR0cHM6Ly9naXN0LmdpdGh1Yi5jb20vbHVpc2xhdmVuYS9mMDY0MjExNzU5ZWUwZjgwNmM4OA==
