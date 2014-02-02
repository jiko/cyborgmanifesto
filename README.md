An Ironic Dream
===========

A Twitter bot, [@anironicdream](https://twitter.com/anironicdream), based on [Donna Haraway's Cyborg Manifesto](http://www.egs.edu/faculty/donna-haraway/articles/donna-haraway-a-cyborg-manifesto/). 

Two versions are included. The one in Python acted as a control. The second, in Go, I started as my fourth attempt. I have not included the code for my first two attempts.

My first attempt in Jabbascript derailed after a sequential clause-by-clause approach proved too difficult for my amatuer parsing skills. My second attempt in Clojure worked for a day but now this happens everytime I do a `lein run`:

    Exception in thread "main" java.lang.IllegalArgumentException: No matching clause: 
      at clojure.data.json$read_json.invoke(json_compat_0_1.clj:23)
      at clojure.data.json$read_json.invoke(json_compat_0_1.clj:18)
      at twitter.callbacks.handlers$get_twitter_error_message.invoke(handlers.clj:85)
      at twitter.callbacks.handlers$response_throw_error.invoke(handlers.clj:52)
      at twitter.callbacks.handlers$handle_response.doInvoke(handlers.clj:115)
      at clojure.lang.RestFn.invoke(RestFn.java:464)
      at twitter.request$get_response_transform$fn__1830.invoke(request.clj:29)
      at twitter.request$execute_request_callbacks.invoke(request.clj:45)
      at twitter.core$http_request.invoke(core.clj:103)
      at twitter.api.restful$statuses_update.doInvoke(restful.clj:56)
      at clojure.lang.RestFn.invoke(RestFn.java:457)
      at app.core$_main.invoke(core.clj:22)
      at clojure.lang.Var.invoke(Var.java:411)
      at user$eval3$fn__5.invoke(NO_SOURCE_FILE:1)
      at user$eval3.invoke(NO_SOURCE_FILE:1)
      at clojure.lang.Compiler.eval(Compiler.java:6619)
      at clojure.lang.Compiler.eval(Compiler.java:6609)
      at clojure.lang.Compiler.eval(Compiler.java:6582)
      at clojure.core$eval.invoke(core.clj:2852)
      at clojure.main$eval_opt.invoke(main.clj:308)
      at clojure.main$initialize.invoke(main.clj:327)
      at clojure.main$null_opt.invoke(main.clj:362)
      at clojure.main$main.doInvoke(main.clj:440)
      at clojure.lang.RestFn.invoke(RestFn.java:421)
      at clojure.lang.Var.invoke(Var.java:419)
      at clojure.lang.AFn.applyToHelper(AFn.java:163)
      at clojure.lang.Var.applyTo(Var.java:532)
      at clojure.main.main(main.java:37)

As far as I can read this, it would seem the library I'm using isn't agreeing with the Twitter API.
