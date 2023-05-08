# graph.c File Reference
---
```
#include <stdio.h>
#include <stdlib.h>
#include "graph.h"
#include "../queue/queue.h"
```

## Functions
---
```
Node * createNode (int v)
Graph * createGraph (int vertices)
void addEdge (Graph *g, int s, int d)
void printGraph (Graph *g)
void free_graph (Graph *g)
void DFS (Graph *graph, int vertex)
void BFS (Graph *graph, int startVertex)
```

## Function Documentation
---
### ◆ addEdge()
```	
>> - void addEdge (Graph * g, int s, int d)	
```

### ◆ BFS()
```
>> void BFS (Graph * graph, int startVertex)	
```

### ◆ createGraph()
```
>> Graph * createGraph (int vertices)	
```

### ◆ createNode()
```
>> Node * createNode (int v)
```

### ◆ DFS()
```
>> void DFS (Graph * graph, int vertex)
```

### ◆ free_graph()
```
>> void free_graph (Graph * g)
```

### ◆ printGraph()
```
>> void printGraph (Graph * g)
```
