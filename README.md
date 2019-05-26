# GeneralNotes

# Starting a Company
* Y-Combinator Lectures
* Business Model Canvas
* Simon Wardley & Wardley Maps
* Ben Hall

# Containerization
* Docker
* Alternatives to docker
* Docker 

# Kubernetes
* Overview
* Tooling
  * k9s https://github.com/derailed/k9s 
  * kubectx https://github.com/ahmetb/kubectx manage contexts
  * kubens https://github.com/ahmetb/kubectx manage namespaces
  * popeye https://github.com/derailed/popeye config linting 
  * stern https://github.com/wercker/stern log management
  * k3s https://k3s.io/ kubernetes for IoT
  * Docker for Desktop ( now contains kubernetes) 
* Orchestration
* ServiceMesh
  * Knative

# Development
* Keep the feedback loop as small as possible
* REPL + test & commit || revert
* Nulls mean keep Redesigning
* Immutability
  * operations to update - return a new object with the new versions.
* Union Types
* Builder Model
#  Testing

# Architecture
* EventStorming
  Albert Brandolini
  * Event Modelling
    Adam Dymitruk
* CQRS
  * Split the model
  * Do the work up front
* CAP Theorem ( Consistentcy, Availability and Partition Tolerance )
* CSP ( Communicating Sequential Processes ) 
* CEP ( complex event processing ) 
  * Reactive Programming (Rx)
  * fits into the the CQRS readmodel update pattern.
* Eventsourcing

# Bigscale 
* Daniel Lemire
* Inverted Indices for Scale
* Lambda Architecture 
  (Batch model + differences from streaming updates merged togteher )
* Kafka
* Cassandra 
  column store
* Druid
  based upon cassandra, but aggregates results from an eventsource
* Mongo - you're probably doing it wrong
  document based
  duplication is good
  joining is BAD
  updates based upon CQRS readmodel pattern
  (ie. background inserts/updates using queue/messagebus fed handlers)

# Security
* Keycloak
* Metron (SIEM) 
  https://metron.apache.org/ 
  
# Web Development
* JAM ( Javascript Api's 

# Languages
* Use better languages 'functional first languages'
  * F# ( .net core is now crazy performant) 
  * golang
  * Clojure
