# desc 'outputs hello to the terminal'
# task :hello do
#   puts "hello from Rake!"
# end

namespace :greeting do
desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'outputs hola to the terminal'
  task :hola do
    puts "hola de Rake!"
  end
end

namespace :db do
  desc 'migrate changes to your database'
  task migrate: :environment do
    Student.create_table
  end

  task :environment do
    require_relative './config/environment'
  end

  desc 'seed the database with some dummy data'
  task seed: :environment do
    require_relative './db/seeds'
end
end

# namespace :pry
desc 'drop into the Pry console'
task console: :environment do
  Pry.start
end

# task :environment do
#   require_relative './config/environment'
# end
# end
