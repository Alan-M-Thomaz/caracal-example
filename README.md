# Caracal Example

This project is a simple Rails application that demonstrates how to
use Caracal to generate MSWord documents in what the library authors
deem idiomatic usage.  You can, of course, implement the library any
way you see fit.  This is merely a suggestion.

Additionally, this project produces a Word document that demonstrates
nearly every configuration option Caracal can manage. As such, the core
team often uses the resulting output for compatibility tests between
the innumerable versions of Word.


## Getting Started

### Web Server

Because this example page includes images, it requires more than one
processing thread. **Please, do not use Webrick.**  Webrick is
single-threaded.  If you try to load the example page using Webrick,
the request will timeout.

We recommend using Puma instead.  The puma gem will be installed
when you `bundle install`.


### Routes

The project is configured to run the example code from the root route.
To generate the file, simply load http://localhost:3000 (or whichever
hostname and port you prefer).
