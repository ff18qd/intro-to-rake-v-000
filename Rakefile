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
  desc 'migrate db'
  task :migrate => :environment do
    Student.create_table
  end

  desc 'add dummy data to db'
  task :seed do
    require_relative './db/seeds.rb'
  end

end


task :environment do
  require_relative './config/environment'
end
