source "http://rubygems.org"

# CoffeeScript
gem "coffee-script"

# Guard
gem "guard"
gem "guard-coffeescript"
gem "guard-copy"
gem "guard-bundler"
gem "guard-livereload"

# Platform
case RUBY_PLATFORM
when /darwin/
    gem "rb-fsevent"
when /win32/
    gem "rb-fchange"
when /linux/
    gem "rb-fchange"
end
