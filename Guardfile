guard 'rspec', :version => 2, :cli => '-c' do
  watch(%r{^spec/.+_spec\.rb})
  watch(%r{^lib/(.+)\.rb})     { |m| "spec/#{m[1]}_spec.rb" }
  watch('spec/spec_helper.rb') { "spec" }
end

guard 'bundler', :notify => true do
  watch('Gemfile')
  watch(/^.+\.gemspec/)
end
