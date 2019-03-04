require_relative 'config/environment.rb'
require "sinatra/activerecord/rake"

desc "starts console"
task :console do
  Pry.start
end

=begin
The model that has_many is considered the parent. 
The model that belongs_to is considered the child. 
If you tell the child that it belongs to the parent, the parent won't know about that relationship. 
If you tell the parent that a certain child object has been added to its collection, 
both the parent and the child will know about the association.

so do this:
  1. rolling_in_the_deep = Song.new(name: "Rolling in the Deep")
  2. adele.songs << rolling_in_the_deep
  3. pop.songs << rolling_in_the_deep
instead of assign artist like this:
  rolling_in_the_deep.artist = "adele"
=end

