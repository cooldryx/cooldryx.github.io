---
layout: post
title: Bundle install
---

Issue
===
When installing __jekyll__ in Ubuntu with `bundle install`, got error message as follows.

>Gem::Installer::ExtensionBuildError: ERROR: Failed to build gem native extension.
>
>        /usr/bin/ruby1.9.1 extconf.rb
>/usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require': cannot load such file -- mkmf (LoadError)
>	from /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require'
>	from extconf.rb:1:in `<main>'
>
>Gem files will remain installed in /tmp/bundler20141030-14370-1ywr1ze/RedCloth-4.2.9/gems/RedCloth-4.2.9 for inspection.
>Results logged to /tmp/bundler20141030-14370-1ywr1ze/RedCloth-4.2.9/gems/RedCloth-4.2.9/ext/redcloth_scan/gem_make.out
>An error occurred while installing RedCloth (4.2.9), and Bundler cannot continue.
>Make sure that `gem install RedCloth -v '4.2.9'` succeeds before bundling.

Solve
===
`sudo apt-get install ruby1.9.1-dev`

Lacking of __ruby-dev__.
