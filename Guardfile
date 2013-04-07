# vim: ft=ruby :

# Watch gemfile
guard 'bundler' do
    watch('Gemfile')
end


# Compile CoffeeScript and copy static content.

guard 'coffeescript', :input => 'source/coffee', :output => 'dist', :all_on_start => true, :bare => true
guard 'copy', :from => 'source/static', :to => 'dist', :verbose => true, :delete => true, :run_at_start => true

guard 'livereload' do
    watch(%r{dist/.*})
end
