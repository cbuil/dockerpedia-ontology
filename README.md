[Dockerpedia Ontology](https://cbuil.github.io/dockerpedia-ontology/release/0.1.0/index-en.html)
===================

The purpose of the [DockerPedia ontology](https://cbuil.github.io/dockerpedia-ontology/release/0.1.0/index-en.html) is to represent software images. The ontology is a simple vocabulary with  prefix docker. The ontology main classes are `docker:Dockerfile`, which is used to build a `docker:SoftwareImage`, which itself is decomposed in `docker:ImageLayers`. Since we aim to track the particular versions of all packages installed in an image, we distinguish the concept `docker:SoftwarePackage` and its respective `docker:PackageVersions`.
We also include the representation of `docker:SoftwareVulnerabilities`, which are crucial to create alerts when comparing or reusing software images. 

We reuse and extend existing ontologies whenever possible. We build on the [Workflow Infrastructure Conservation Using Semantics ontology](http://vocab.linkeddata.es/wicus/wicus/) (WICUS with prefix `wicus`), an OWL ontology network that represents the main concepts of a computational infrastructure. WICUS contains terminology for describing computational scientific experiments, including their software, hardware and computing resources; and we align our terminology to existing classes and properties. A `docker:Dockerfile` is defined as subclass of the more generic `wicus:DeploymentScript`, as each Docker file contains the set of actionable steps to be carried out during the deployment of the container.

### License

MIT License, Copyright © 2021 <DockerPedia>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.