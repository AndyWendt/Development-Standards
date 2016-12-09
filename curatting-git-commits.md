# Curatting Git Commits

## Committing to Great Communication

### The Process


#### Separate subject from body with a blank line

*Do not* do this:
 
```
This Is The Subject
This is the body.  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean lacinia bibendum nulla sed consectetur. Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Aenean lacinia bibendum nulla sed consectetur. Cras mattis consectetur purus sit amet fermentum. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Praesent commodo cursus magna, vel scelerisque nisl consectetur et.Donec sed odio dui. Donec id elit non mi porta gravida at eget metus. Vestibulum id ligula porta felis euismod semper. Donec id elit non mi porta gravida at eget metus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean lacinia bibendum nulla sed consectetur.

```
 
Do this: 


```
This is the subject

This is the body.  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean lacinia bibendum nulla sed consectetur. Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Aenean lacinia bibendum nulla sed consectetur. Cras mattis consectetur purus sit amet fermentum. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Praesent commodo cursus magna, vel scelerisque nisl consectetur et.Donec sed odio dui. Donec id elit non mi porta gravida at eget metus. Vestibulum id ligula porta felis euismod semper. Donec id elit non mi porta gravida at eget metus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean lacinia bibendum nulla sed consectetur.

```


#### Limit the subject line to 50 characters

*Do not* do this:

```
This is the the subject that goes on forever and it is really several runon sentences rolled into one just because I did not put any thought into what I was going to write since I was in a rush and my hamster escaped so therefore I could not shorten this subject so that it could be understandable

...body...
```

Do this: 


```
This is a summary of the commit

...body...
```


#### Capitalize the subject line and the body

*Do not* do this:

```
my PET gerbil esCapEd fRoM hIs laIr

this is the body.  Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Curabitur blandit tempus porttitor. Praesent commodo cursus magna, vel scelerisque nisl consectetur et. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum.Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Donec sed odio dui. Donec sed odio dui. Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Sed posuere consectetur est at lobortis. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.
```

Do this: 

```
My pet gerbil escaped from his lair


This is the body.  Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Curabitur blandit tempus porttitor. Praesent commodo cursus magna, vel scelerisque nisl consectetur et. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum.Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Donec sed odio dui. Donec sed odio dui. Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Sed posuere consectetur est at lobortis. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.
```


#### Do not end the subject line with a period

*Do not* do this:

```
Raccooons make great pets.

...body...
```

Do this: 

```
Raccoons make great pets

...body...
```

#### Use the imperative mood in the subject line

This is defining what is to be accomplished with the commit.  It should be read with the prefix: `If applied, this commit will <subject>`

 For example: _If applied, this commit will_ `add getting started documentation`

*Do not* do this:

```
Added getting started documentation

...body...
```

Do this: 

```
Add getting started documentation

...body...
```


#### Wrap the body at 72 characters

PHPStorm and other git clients do this automatically.  From the commandline, you will need to configure your editor to wrap at 72 characters.


#### Use the body to explain what and why vs. how


*Do not* do this:

```
Change User Table to Include Timestamps

Added timestamps by using laravel's timestamps migration method and by running `php artisan migrate`.
Created a new migration to do this.   Also changed a recursive function just because it needed to be 
"fixed."

When I was looking at our documentation for migrations, I noticed that the reference to the how to add 
soft deletes was incorrect.   I updated all of the models to use soft deletes by using the soft delete 
trait.   

Hopefully this doesn't break anything.  
```


Do not do this: 

```
Change User Table to Include Timestamps

Add `created_at` and `updated_up` to users table.  We need to know when 
we or the users update their account or when we create the account.  
This will allow us todisplay this information on their dashboard.    
```



## Resources


* http://chris.beams.io/posts/git-commit/#capitalize
* https://git-scm.com/book/en/v2
* https://www.git-scm.com/book/en/v2/Distributed-Git-Contributing-to-a-Project#Commit-Guidelines
* http://alistapart.com/article/the-art-of-the-commit
* https://keithhamilton.gitbooks.io/features-commits-pull-requests/content/crafting-a-good-commit.html
* https://brigade.engineering/the-secrets-to-great-commit-messages-106fc0a92a25#.chatrpmj9
