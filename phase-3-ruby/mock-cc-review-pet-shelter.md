# Phase 3 Ruby & Active Record Study Guide

## Goals
- be able to articulate the general requirements for the Phase 3 code challenge
- be able to complete all the deliverables for the Pet Shelter mock challenge

## Review: connecting Ruby concepts to Active Record
- What is a Ruby class? An instance?
- In Active Record, a table corresponds to a Ruby ___________ and a row corresponds to ___________. Each table column corresponds to a __________.
- What is a foreign key?
- What is a join table?
- What is a many-to-many relationship?
- A great resource for learning object-oriented Ruby: ( [slides](https://docs.google.com/presentation/d/1q8aHtZuveTKJLZql6V4YRxbIwBreEcO6Ep-A5oK1UOA/edit#slide=id.p) )


## What's needed to pass the code challenge
1. Build tables with migrations (note that the table, terminal command, and migration filename all use the plural)
	```
	# terminal commands:

	$ rake db:create_migration NAME=create_students
	
	$ rake db:migrate
	
	$ rake db:seed
	```
	```
	# example migration
	
	20230206114821_create_students.rb |
	-----------------------------------
	class CreateStudents < ActiveRecord::Migration[7.0]
	  def change
		create_table :students do |t|
		  t.string :first_name
		  t.string :last_name
		  t.integer :grade_point_avg
		  t.integer :grad_year
		end
	  end
    end
	```
2. Set up your associations so the classes can access each other using Active Record macros (note which ones must be plural vs singular):
	```ruby
	has_many: :xs
	belongs_to: :y
	has_many: :zs, through: :xs
	```
3. Build custom methods to manipulate/sort your data

	```ruby
	# use an instance method when you want your method to do stuff to one specific instance
	# examples: 
	# - updating values for that instance
	# - sorting things related to that specific instance

	def my_instance_method
		...
	end

	
	# use a class method when you want your method to do something that requires an overview of all the items in that class
	# examples: 
	# - sorting
	# - finding
	# - comparing

	def self.my_class_method
		...
	end

	
	# helpful ruby built-in methods for sorting, finding, etc
	# learn what they do and how to use them! find more!

	.max_by
	.min_by
	.count
	.average
	.order
	.reverse
	.last
	.first
	.to_i
	.to_s
	.where
	.find
	.find_by
	```


## Step by step: Pet Shelter Mock CC

### [github link](https://github.com/brewchetta/phase-3-practice-code-challenge-animal-shelter)  — fork it 

I recommend NOT coding along during this walk-through. Instead, focus on making sure you understand each step by asking questions and trying to anticipate what the next step should be.

I DO recommend completing this mock CC on your own from a blank slate as soon as possible, and then again tomorrow (or a similar one, like the ones below)

[Aliens Among Us](https://github.com/brewchetta/phase-3-practice-code-challenge-aliens-among-us)

[Karaoke Maniacs](https://github.com/brewchetta/phase-3-ar-practice-karaoke-mania) (more challenging)