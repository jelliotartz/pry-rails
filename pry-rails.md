# Pry for Rails!

### what does it do?

Pry is a powerful alternative to the standard IRB shell for Ruby, which has more benefits than IRB. e.g, you can cd into objects, call methods, adjust variables. It can also be used as a debugger, letting you step into your code by adding binding.pry into your codebase at the desired break point.

### some pry resources:

[Github](https://github.com/pry/pry)

[Github Pry wiki](https://github.com/pry/pry/wiki)

### How to install: 

gemfile: 

`gem 'pry-rails'`

`gem pry jazz-hands`: a bundle of pry gems, including bye-bug and cool line.



### Some shell commands available via pry-rails

**ls -m** list methods available to an object   

**show-doc** see documentation for methods available to objects


**find-routes**
```ruby
Routes for ArticlesController
--
index GET /  [root]
index GET /articles(.:format)  [articles]
create POST /articles(.:format)
new GET /articles/new(.:format)  [new_article]
edit GET /articles/:id/edit(.:format)  [edit_article]
show GET /articles/:id(.:format)  [article]
update PATCH /articles/:id(.:format)
update PUT /articles/:id(.:format)
destroy DELETE /articles/:id(.:format)
```


### Pry can also be used as a debugger!

####PLUG-INS:

`gem 'pry-byebug'`: Adds step, next, finish and continue commands and breakpoints to Pry using byebug.
	-step: Step execution into the next line or method. Takes an optional numeric argument to step multiple times.
	-next: Step over to the next line within the same frame. Also takes an optional numeric argument to step multiple lines.
	-finish: Execute until current stack frame returns.
	continue: Continue program execution and end the Pry session.
	-up: Moves the stack frame up. Takes an optional numeric argument to move multiple frames.
	-down: Moves the stack frame down. Takes an optional numeric argument to move multiple frames.
	-frame: Moves to a specific frame. Called without arguments will show the current frame.
	-break: Set a new breakpoint from a line number in the current file, a file and line number, or a method.

use **whereami** to figure out... where you are

setting pry up as your RAILS CONSOLE- once it's added into gemfile, it replaces IRB as the default console. 

`pry cool line`

```ruby 
h = {x: "hello"}
{
    :x => "hello"
}
```






