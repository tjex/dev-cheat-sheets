Bulk updating bookmarks: all bms with tag 'sa' also get tag 'py'
`bkmr update -t py $(bkmr search -t sa --np)`

Bulk updating bookmarks: all bms with tag 'gh' should have 'git' removed
`bkmr update -n git $(bkmr search -t gh --np)`

Tagging and usage system to follow when using bkmr (https://github.com/sysid/bkmr)
so that it doesn't become unwieldy.

> career
> company
> culture (catch all term - ie for a culture publication)
>     - book
>     - music
>     - art
>     - film
>     - events
> education
> hardware
> lifestyle (catch all term)
>     - travel
>     - health
>     - sport
>     - food
> local
> programming
> project -> p/projname (all bookmarks with this tag can then be programatically deleted when project is done)
> ref
> software
> tech
> work -> w/companyx

Further sorting happens by giving a descriptive title and comment. 
Then SQL queries can be made against the db in conjunction with tags.
This also limits the pressure of considering to add an extra tag or not, 
and increases the ability to find desired bookmarks. e.g.: 

`bkmr search -t tech 'go AND library'`


