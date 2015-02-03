Framework Ideas
---------------

This is a list of potential web frameworks to use. Although it assumes we will be
making a website for the frontend, all of these options should allow for providing
a REST-ful service if required, for communication with Android/iOS devices (or
anything else really).

It is also important to note that each team might be affected differently by each
choice. The interface team will be primarily concerned with HTML5, CSS and Javascript,
and potentially the template language of the chosen framework. The data team will be
primarily concerned with how models are handled in the chosen framework, along with
the provided ORM.

- - - -

### [Spring.io] ([spring-boot])
- Main Language: Java
- Main Template Language: [Thymeleaf]

Advantages:
- We all should be familiar with Java
- Spring.io's subprojects should offer most of the desired functionality
- Java is statically typed, eliminating potential runtime errors

Disadvantages:
- Not as convention-based as the other options
- JPA can make ORM kinda complex in comparison to ActiveRecord
- Java is statically typed, meaning the server will have to be rebuilt for
  each modification even if just to test something
- Much more code will be required in comparison to ruby/javascript

- - - -

### [Rails]
- Main Language: Ruby
- Main Template Languages: ERB, [Haml]

Advantages:
- Has a lot of needed stuff bundled in, including ORM for database interaction (via [ActiveRecord])
- Convention over configuration (everything has its place)
- Extendable via gems

Disadvantages:
- Those who don't know ruby would need to learn it
- Might not play well on Windows/OSX, thus virtualization may be required
  - Tools like [Vagrant] could make this painless and actually convenient, but
    some machines/laptops may not be powerful enough to host a virtual machine

- - - -

### [Node] + [Express]
- Main Language: Javascript
- Main Template Language: [Jade]

Advantages:
- As with Rails, a lot of stuff is bundled in
- Extendable via middleware, node packages, bower packages

Disadvantages:
- Those who don't know javascript would need to learn it
- Same potential virtualization issues as mentioned above for Rails
- Node's single-threaded nature can cause it to suffer under heavy load

- - - -

### Other options
A few other options that I don't personally have much experience with:
- Python + [Django]
- PHP + [Laravel]
- Node + [Meteor]

[ActiveRecord]:http://guides.rubyonrails.org/active_record_querying.html
[Django]:https://www.djangoproject.com/
[Express]:http://expressjs.com/
[Haml]:http://haml.info/
[Jade]:http://jade-lang.com/
[Laravel]:http://laravel.com/
[Meteor]:https://www.meteor.com/
[Node]:https://nodejs.org/
[Rails]:http://rubyonrails.org/
[Spring.io]:https://spring.io/
[spring-boot]:http://projects.spring.io/spring-boot/
[Thymeleaf]:http://www.thymeleaf.org/
[Vagrant]:https://www.vagrantup.com/
