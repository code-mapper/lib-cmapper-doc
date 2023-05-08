# linked_list.c File Reference
---
```
#include <stdlib.h>
#include "list.h"
```

## Functions
---
```
void list_init (struct list *list)
int list_is_empty (struct list *list)
size_t list_len (struct list *list)
void list_push_front (struct list *list, struct list *elm)
struct list * list_pop_front (struct list *list)
struct list * list_find (struct list *list, int value)
int list_is_sorted (struct list *list)
void list_insert (struct list *list, struct list *elm)
void list_rev (struct list *list)
```

## Function Documentation
---
### ◆ list_find()
```
>> struct list* list_find (struct list * list, int value)
```

### ◆ list_init()
```
>> void list_init (struct list * list)
```

### ◆ list_insert()
```
>> void list_insert (struct list * list, struct list * elm)
```

### ◆ list_is_empty()
```
>> int list_is_empty (struct list * list)
```

### ◆ list_is_sorted()
```
>> int list_is_sorted (struct list * list)
```

### ◆ list_len()
```
>> size_t list_len (struct list * list)
```

### ◆ list_pop_front()
```
>> struct list* list_pop_front (struct list * list)
```

### ◆ list_push_front()
```
>> void list_push_front (struct list * list, struct list * elm)
```

### ◆ list_rev()
```
>> void list_rev (struct list * list)
```
