task :default => [:greet_user]

desc "Print a friendly greeting"
task :greet do
  puts "Hello There"
end

desc "Prints the current time"
task :time do
  puts Time.now
end

desc "Asks a user for their name and greets them"
task :greet_user do
  name = ''
  STDOUT.puts "What is your name?"
  name = STDIN.gets.chomp
  puts "Hello, #{name}"
end

desc "Prints the favorite food env variable"
task :print_favorite_food do
  puts "Your favorite food is #{ENV["food"]}."
end

task :first do
  puts "First!"
end

task :second => :first do
  puts "Second!"
end

namespace :hedwig do
  task :wake_up do
    puts "I put on some make-up"
    puts "And turn on the tape deck"
  end

  task :get_dressed => :wake_up do
    puts "And pull the wig back on my head"
    puts "Suddenly I'm Miss Midwest Midnight checkout queen"
  end

  task :finish_day => :get_dressed do
    puts "Until I head home"
    puts "And I put myself to bed"
  end
end

namespace :greeting do
  desc "Say Hello"
  task :hello do
    puts "Hello there"
  end

  desc "Say Howdy"
  task :howdy do
    puts "Howdy Partner"
  end
end


