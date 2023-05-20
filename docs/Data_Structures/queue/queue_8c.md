## Documentation Files
---
```
#include <stdlib.h>
#include <stdio.h>
#include "queue.h"
```

### Qu'est ce qu'une file ?
Une file est une structure de données qui permet de stocker des éléments de façon ordonnée. Les éléments sont ajoutés à la fin de la file et retirés au début de la file. On parle de structure de données FIFO (First In First Out) ou PEPS (Premier Entré Premier Sorti).

###  Definition de la file
---
```
int items [SIZE]
int front
int rear
```

###  Definition des attributs
---
#### ◆ front
```	
>> int front
```

#### ◆ items
```	
>> int items[SIZE]
```

#### ◆ rear
```
>> int rear
```

### Data Structures
---
```
struct QUEUE
```

### Type Definitions
---
```
typedef struct QUEUE Queue
```

### Code Source
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

### Definition des fonctions
---
#### ◆ createFillQueue()
```
>> Queue* createFillQueue (int n)
```

#### ◆ createQueue()
```
>> Queue* createQueue ()
```

#### ◆ dequeue()
```
>> int dequeue (Queue * q)
```

#### ◆ enqueue()
```
>> void enqueue (Queue * q, int value)
```

#### ◆ isEmpty()
```
>> int isEmpty (Queue * q)
```

#### ◆ printQueue()
```
>> void printQueue (Queue * q)
```

