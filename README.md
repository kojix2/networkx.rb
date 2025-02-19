# NetworkX.rb

[NetworkX](https://networkx.github.io/) is a very popular Python library, that handles various use-cases of the Graph Data Structure.  
This project intends to provide a working alternative to the Ruby community, by closely mimicing as many features as possible. 

## List of contents

- [Installing](#installing)
- [Document](#document)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)

## Installing

- Clone the repository or fork
  - Clone this repository with `git clone https://github.com/sciruby-jp/networkx.rb.git`
  - or You can fork and do clone it.
- Navigate to networkx with `cd networkx.rb`
- Install dependencies with `gem install bundler && bundle install`

```ruby
require 'networkx'

g = NetworkX::Graph.new
g.add_edge('start', 'stop')
``` 

## Document

You can read [Document](https://sciruby-jp.github.io/networkx.rb/) for this library.

## Roadmap

Quite easily, any networkx user would be able to understand the number of details that have been implemented in the Python library. As a humble start towards the release of v0.1.0, the following could be the goals to achieve :

- `Node` : This class should be capable of handling different types of nodes (not just `String` / `Integer`).  
   A possible complex use-case could be XML nodes.

- `Edge` : This class should be capable of handling different types of edges.  
  Though a basic undirected Graph doesn't store any metadata in the edges, weighted edges and parametric edges are something that need to be handled.

- `Graph` : The simplest of graphs.  
  This class handles just connections between different `Node`s via `Edge`s.

- `DirectedGraph` : Inherits from `Graph` class.  
  Uses directions between `Edge`s.

## Contributing

Your contributions are always welcome!  
Please have a look at the [contribution guidelines](CONTRIBUTING.md) first. :tada:

## License

The MIT License 2017 - [Athitya Kumar](https://github.com/athityakumar).   
Please have a look at the [LICENSE.md](LICENSE.md) for more details.
