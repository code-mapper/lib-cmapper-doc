# queue.c File Reference
---
```
#include <stdlib.h>
#include <stdio.h>
#include "queue.h"
```

## Data Structures
---
```
struct QUEUE
```

## Type Definitions
---
```
typedef struct QUEUE Queue
```

## Code Source
---
```
#ifndef QUEUE_H_
#define QUEUE_H_
 
#define SIZE 40
 
typedef struct QUEUE {
  int items[SIZE];
  int front;
  int rear;
}Queue;
 
 
Queue* createQueue();
void enqueue(Queue* q, int);
int dequeue(Queue* q);
Queue* createFillQueue(int n);
void display(Queue* q);
int isEmpty(Queue* q);
void printQueue(Queue* q);
 
 
#endif
```

## Function Documentation
---
### ◆ createFillQueue()
```
>> Queue* createFillQueue (int n)
```

### ◆ createQueue()
```
>> Queue* createQueue ()
```

### ◆ dequeue()
```
>> int dequeue (Queue * q)
```

### ◆ enqueue()
```
>> void enqueue (Queue * q, int value)
```

### ◆ isEmpty()
```
>> int isEmpty (Queue * q)
```

### ◆ printQueue()
```
>> void printQueue (Queue * q)
```

