require 'asciidoctor'
require 'em/pure_ruby'

guard 'shell' do
  watch(/^README\.adoc$/) {|m|
    Asciidoctor.convert_file 'README.adoc', safe: :unsafe
  }
end

guard 'livereload' do
  watch(%r{^.+\.(css|js|html)$})
end