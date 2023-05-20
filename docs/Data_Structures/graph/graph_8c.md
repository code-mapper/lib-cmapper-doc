## Documentation Graphes
---
```
#include <stdio.h>
#include <stdlib.h>
#include "graph.h"
#include "../queue/queue.h"
```

### Definition du graphe
---
```
int  numVertices
int* visited
struct NODE** adj
```
### Documentation des attributs
---
#### ◆ adj
```
>> struct NODE** adj
```

#### ◆ numVertices
```
>> int numVertices
```
#### ◆ visited
```
>> int* visited
```

### Code Source
---
```
#ifndef GRAPH_H_
#define GRAPH_H_
 
 
typedef struct NODE {
    int vertex;
    struct NODE* next;
}Node;
//struct node* createNode(int v);
 
typedef struct GRAPH {
    int numVertices;
    int *visited;
    struct NODE** adj;
}Graph;
 
 
Node* createNode(int v);
Graph* createGraph(int vertices);
void addEdge(Graph* graph, int s, int d);
void printGraph(Graph* graph);
void free_graph(Graph* graph);
void DFS(Graph* graph, int vertex);
void BFS(Graph* graph, int startVertex);
 
#endif
```

### Documentation des fonctions
---
#### ◆ addEdge()
```	
>> void addEdge (Graph * g, int s, int d)	
```

#### ◆ BFS()
```
>> void BFS (Graph * graph, int startVertex)	
```

#### ◆ createGraph()
```
>> Graph * createGraph (int vertices)	
```

#### ◆ createNode()
```
>> Node * createNode (int v)
```

#### ◆ DFS()
```
>> void DFS (Graph * graph, int vertex)
```

#### ◆ free_graph()
```
>> void free_graph (Graph * g)
```

#### ◆ printGraph()
```
>> void printGraph (Graph * g)
```
