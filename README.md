# Twitter Example

A Twitter bot example in Clojure

## Step-by-step Tutorial

To get familiar with the programming language Clojure and the development workflow, first off follow the step-by-step tutorial [Twitter Bot Example in Clojure](http://howistart.org/posts/clojure/1). Skip the Emacs and testing steps in the tutorial.

Create a project folder for your twitter bot in the `projects` directory in the clojure setup in Vagrant. This will be your working directory.

Alternatively to the step-by-step tutorial you can download the finished project [lemmings-io/01-twitter-example](https://github.com/lemmings-io/01-twitter-example/archive/master.zip) and copy it into the `/lemmings/clojure/projects` directory in your virtual machine setup.

## Setting up the development environment for usage in the VM

Create a file called "profiles.clj" in your working directory.

```
{:dev {:env {:app-consumer-key "<REPLACE>"
             :app-consumer-secret "<REPLACE>"
             :user-access-token "<REPLACE>"
             :user-access-secret "<REPLACE>"}}}
```

## Start the twitter bot in the VM

`lein trampoline run` to start the local server.

## Test if your bot tweets

Running `(status-update)` in the nREPL sends a status update through your twitter account.

## Credit

This example is based on the [Twitter Bot Example in Clojure](http://howistart.org/posts/clojure/1) by [Carin Meier](https://twitter.com/carinmeier).

## License

Copyright © 2017

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.
