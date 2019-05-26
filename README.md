# GeneralNotes

# Starting a Company
* Y-Combinator startup school : https://www.youtube.com/playlist?list=PLQ-uHSnFig5NVnJ_cLWM7dLuMQRDeekoX
* Business Model Canvas : https://en.wikipedia.org/wiki/Business_Model_Canvas 
* Simon Wardley & Wardley Maps
* Ben Hall
  * katacoda https://www.katacoda.com/

# Containerization
* Docker
* Alternative to docker KKT
* Docker Swarm (docker compose)

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
  * Helm https://helm.sh package management for kubernetes
  * Draft https://draft.sh make k8s projects
  * Kompose https://kompose.io use docker-compose with kubernetes
* Orchestration
* ServiceMesh
  * Istio
  * Envoy
  * Knative
  
  https://dzone.com/articles/50-useful-docker-tools
  https://dzone.com/articles/50-useful-kubernetes-tools

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

# Workflow
* gitops
* gitlab

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
* JAM Stack https://jamstack.org/ JavaScript, reusable APIs, and prebuilt Markup 

# Languages
* Use better languages 'functional first languages'
  * F# ( .net core is now crazy performant) 
  * golang
  * Clojure
