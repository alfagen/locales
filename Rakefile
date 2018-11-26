task :check_yaml do
  require 'psych'

  Dir['./**/*.yml'].each do |file|
    begin
      Psych.load_file(file)
      puts "#{file} - ok"
    rescue Psych::SyntaxError => ex
      puts "error: #{ex}"
    end
  end
end
