task :default do
  require 'json'
  sh "parse-hocon hocon/style.conf > htdocs/style.json"
  style = JSON.parse(File.read('htdocs/style.json'))
  File.write('htdocs/style.json', JSON.pretty_generate(style))
  sh "gl-style-validate htdocs/style.json"
end
task :plain do
  require 'json'
  sh "parse-hocon hocon-plain/style.conf > htdocs/clearmap-plain.json"
  style = JSON.parse(File.read('htdocs/clearmap-plain.json'))
  File.write('htdocs/clearmap-plain.json', JSON.pretty_generate(style))
  sh "gl-style-validate htdocs/clearmap-plain.json"
end
task :dark do
  require 'json'
  sh "parse-hocon hocon-dark/style.conf > htdocs/clearmap-dark.json"
  style = JSON.parse(File.read('htdocs/clearmap-dark.json'))
  File.write('htdocs/clearmap-dark.json', JSON.pretty_generate(style))
  sh "gl-style-validate htdocs/clearmap-dark.json"
end
task :gray do
  require 'json'
  sh "parse-hocon hocon-gray/style.conf > htdocs/clearmap-gray.json"
  style = JSON.parse(File.read('htdocs/clearmap-gray.json'))
  File.write('htdocs/clearmap-gray.json', JSON.pretty_generate(style))
  sh "gl-style-validate htdocs/clearmap-gray.json"
end



