task :check_yaml do
  require 'yaml'

  Dir['./**/*.yml'].each do |file|
    begin
      YAML.load_file(file)
      puts "#{file} - ok"
    rescue Exception
      puts "error: #{$!}"
    end
  end
end
