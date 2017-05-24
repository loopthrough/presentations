Potential topics
===============

* Short about me
** Why this talk, I work on a project with Golang backend
** I have seen that many people would like to try it, but it is not a go to tool for their orgnisations.

* Couple of notes
** Not a comparison, but you'll certainly be able to relate some facts
** it depends on your case

* Many angles from which programming language affects development
* Designed for scaling both your product and the team
* Meant to replace C++ but is affecting Python more in practice. YouTube is rewritten in Go as fara s I've read some time ago.
* Rob Pike, Ken Thompson / Unix, UTF-8, Plan9, Brad Fitzpatrick memcached
* Released 2009, now in version 1.8

* What is specific out with Go lang
** Simplicity/Conservativism as design principle, somewhat towards extreme.
** Combination of low-level power and high level features
** Pragmatism
** It doesn't look like a language of the modern age.

* Simple but effective type system
** Statically typed
** Type inference
** Structured typing, not nominal
** And you can escape it with "interface{}"
** Reflection is not the strongest feature.
** It is too simple for some things. No generics is a running complain since release.

* Concurrency primitives
** Goroutines with typed channels for communication and synchronisation.
** Lightweight threads on top of native OS threads.
** Share memory by communicating, don't communicate by sharing memory.
** Channels are blocking and are mean to synchronise concurrent goroutines.
** It is implementation of CSP concurrency model (Communicating Sequetial Processes)

* Concurrency is not parallelism
** If it will execute in parallel depends on many other things.
** You have to design your work chunks so that they can be executed in parallel.
** Scheduler is improved continuously to run better on multiple cores.

* Compiles to a static binary
** No dependencies on running machine, great from containers.
** Compiles pretty fast.
** As it is compiled is fast.


* Why would you consider it for your next project.
** Good all-around tool which would allow you to expand over time
*** Command-line tools
*** server-rendered HTML apps
*** APIs
*** small services
** Incredibly easy to pick-up but can be misleading in moments.
** Language comes with own HTTP server, supporting HTTP/2
** Language comes with API for implementing simple handling of HTTP requests.
*** Number of frameworks built on top but for lot of cases it is not really needed.
** Testing is quite easy, testing framework provided.
** First class UTF-8, special type for Unicode code points (runes)
** Provides testing framework
** Provide benchmarking framewrk
** Provides decent profiling and tracing tools.
** Has own HTTP server with support for HTTP/2
** Templating libraries for text and html content.
*** Escaping content by default, can be turned of on particular values.





** Pragmatic tool for getting things done, not to learn much about programming.
** Incredibly easy to pick up.
** Particularly good for API development.
* Promoting some principles and habits by engineers.
*** A bit opinionated
*** packages are picked directly from the version control. Only recently package managers to control version fixing.
** encourages use of "go fmt" tool to format code same across community.
** As it is quite simple, it is easy to read code of any library and implementation.
*** This is interesting as a feature.
** Only recently package management tools started emerging.
** Explicit and immediate error handling
** Testing
** It has though phylosophy of small, composed libraries and packages instead of big monolythical frameworks.
*** That makes it more oriented towards custom development than run-off-the-mill projects.
*** It requires more skilled engineers as well to manage the additional complexities of composition.
* Explicit error handling.
* Statically typed
** Type inference makes types not come into your way too muc
** Escape from the type system by interface{}
** Structured typing
** No generics, means you need to implement both StringSet and IntSet.
** Gives good usability on working with JSON over HTTP together with encoding/decoding of JSON.
* Concurrency, goroutines
* UTF-8 support with Unicode code points (runes) as a data type.
** Source code is UTF-8 so you can use your UTF-8 symbols
** Share data by communicating, don't communicate by sharing data.
** Communication over blocking, potentially buffered channels makes synchronisaiton easier.
* Statically linked.
** Great for the containers, just put binary and no dependencies problem.
* Separation of data from functions
* Good combination of lowe level and high-level functionalities
* Passing is always by value, but you can chose of value copy or reference copy
* net/http package
** starts goroutine for each requests
** Interface for middlewards to inject pre- or post-request.
** net/httptest package
** HTTP/2
** Brad Fitzpatrick, memcached, LiveJournal
* text/template, html/template
** Recompiled in run-time, great for development speed.
*** Can be turned off in production
** Safe and escaped by default with options for escaping the safety.
* Testing
* Compilation is very fast
* Tooling
** Good profiling tools, goroutine tracing.
** AST is simple and allows for teams to add tooling as they need, it is not magic.
* Packages
** Web Frameworks, plenty
** Templating included
* Community, live and vibrant Docker, Kubernetes, OpenShift
* Negative aspects
** Not for people with a flare for software design, higher level abstractions.
** Simple type system
* Link to survey results for the year 2016 - [Go survery results](https://blog.golang.org/survey2016-results)
