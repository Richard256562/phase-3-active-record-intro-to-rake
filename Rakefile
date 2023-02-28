namespace :db do
  desc 'migrate changes to your database'
  task migrate: :environment do
    Student.create_table
  end
end
task :environment do
  require_relative './config/environment'
end

namespace :db do
  desc "Seed the database with sample data"
  task seed: :environment do
    Student.create_table
  end
end

desc 'drop into the Pry console'
task console: :environment do
  Pry.start
end