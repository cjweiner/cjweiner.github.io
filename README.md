cjweiner.github.io
==================


I am trying to run my Github-pages website locally. I have it running on another machine that is using Ruby 2.1.0 on Windows x64. Today I wanted to run locally on my home machine that is running Ruby 2.2.0. I pulled my repo locally, ran `bundle install` after a few issues with nokogiri I was able to get through a clean `bundle install`. I then proceeded to run the command `bundle exec jekyll serve -w`. Upon running this command I receive the following errors:

    /Users/<me>/.rvm/gems/ruby-2.2.0@global/gems/commander 4.1.6/lib/commander/runner.rb:385:in block in require_program': program version required (Commander::Runner::CommandError)
        from /Users/<me>/.rvm/gems/ruby-2.2.0@global/gems/commander-4.1.6/lib/commander/runner.rb:384:in `each'
        from /Users/<me>/.rvm/gems/ruby-2.2.0@global/gems/commander-4.1.6/lib/commander/runner.rb:384:in require_program'
        from /Users/<me>/.rvm/gems/ruby-2.2.0@global/gems/commander-4.1.6/lib/commander/runner.rb:52:in run!'
        from /Users/<me>/.rvm/gems/ruby-2.2.0@global/gems/commander-4.1.6/lib/commander/delegates.rb:8:in run!'
        from /Users/<me>/.rvm/gems/ruby-2.2.0@global/gems/commander-4.1.6/lib/commander/import.rb:10:in block in <top (required)>'
    /Users/<me>/.rvm/gems/ruby-2.2.0/gems/safe_yaml-1.0.3/lib/safe_yaml/load.rb:43:in <module:SafeYAML>': undefined method tagged_classes' for Psych:Module (NoMethodError)
        from /Users/<me>/.rvm/gems/ruby-2.2.0/gems/safe_yaml-1.0.3/lib/safe_yaml/load.rb:26:in <top (required)>'
        from /Users/<me>/.rvm/gems/ruby-2.2.0/gems/safe_yaml-1.0.3/lib/safe_yaml.rb:1:in require'
        from /Users/<me>/.rvm/gems/ruby-2.2.0/gems/safe_yaml-1.0.3/lib/safe_yaml.rb:1:in <top (required)>'
        from /Users/<me>/.rvm/gems/ruby-2.2.0/gems/jekyll-1.5.1/lib/jekyll.rb:21:in require'
        from /Users/<me>/.rvm/gems/ruby-2.2.0/gems/jekyll-1.5.1/lib/jekyll.rb:21:in <top (required)>'
        from /Users/<me>/.rvm/gems/ruby-2.2.0/gems/jekyll-1.5.1/bin/jekyll:7:in require'
        from /Users/<me>/.rvm/gems/ruby-2.2.0/gems/jekyll-1.5.1/bin/jekyll:7:in <top (required)>'
        from /Users/<me>/.rvm/gems/ruby-2.2.0/bin/jekyll:23:in load'
        from /Users/<me>/.rvm/gems/ruby-2.2.0/bin/jekyll:23:in <main>'
        from /Users/<me>/.rvm/gems/ruby-2.2.0/bin/ruby_executable_hooks:15:in eval'
        from /Users/<me>/.rvm/gems/ruby-2.2.0/bin/ruby_executable_hooks:15:in <main>'