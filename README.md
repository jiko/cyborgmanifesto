An Ironic Dream
===========

A Twitter bot, [@anironicdream](https://twitter.com/anironicdream), based on [Donna Haraway's Cyborg Manifesto](http://www.egs.edu/faculty/donna-haraway/articles/donna-haraway-a-cyborg-manifesto/) ([alternate link](http://wayback.archive.org/web/20120214194015/http://www.stanford.edu/dept/HPS/Haraway/CyborgManifesto.html)). 

Go code yanked from the [Codewalk Markov chain example](http://golang.org/doc/codewalk/markov/) and the [twittergo tweet example](https://github.com/kurrik/twittergo-examples/blob/master/tweet/main.go).

To use this bot, you need a four-line file called `CREDS` in the directory where you run the bot. `CREDS` must contain your Consumer Key, Consumer Secret, Access Token, and Access Token Secret, in that order, separated by new lines. To get those visit https://dev.twitter.com. To run the bot, use standard in, so on a Unix system:

  cyborgmanifesto < aCyborgManifesto.txt

I'm new to Go, but I think if you clone this repo and run `go install` your should get an executable with the name of this repository, unless you changed the name when you cloned it. If you `go get github.com/jiko/cyborgmanifesto` and then `go install github.com/jiko/cyborgmanifesto` you should have a `cyborgmanifesto` executable in `$GOPATH/bin`. [How to Write Go Code](http://golang.org/doc/code.html), and the Go documentation in general, clarifies matters well.
