##How to Add a New Column to a SQL in Rails

Here's the process for adding a table column in SQLite in a Rails app:

1. add new item in the model `attr_accessible :reviews` where 'reviews' is the column name 
2. create new table column in terminal `rails g migration add_column_reviews_to_bands` where 'bands' is the model name <b>-- Note: the model name is plural --</b>
3. go into the migration file & inside the new change method & add: `add_column :bands, :reviews, :string`
4. on the command line `rake db:migrate`
5. update code in controller/view/whatever to suit new column

That should do it!