```puml
@startuml
node "Kubernetes Cluster" {

    node "Node 1" {
        node "Pod 1" as pod1 {
            component "Container 1" as container111
            component "Container 2" as container112
        }
        node "Pod 3" as pod3 {
            component "Container 1" as container131
        }
    }

    node "Node 2" {
        node "Pod 3" as pod2 {
            component "Container 1" as container231
            component "Container 2" as container232
        }
    }

}
@enduml
```