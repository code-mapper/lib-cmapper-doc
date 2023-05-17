## Documentation listes chainées
---
```
#include <stdlib.h>
#include "list.h"
```

## list Struct Reference
---

```
#include <linked_list.h>
```

### Data Fields
---
```
struct list * 	next
int data
```

### Field Documentation
---
#### ◆ data
```	
>> int data
```

#### ◆ next
```
>> struct list* next

### Data Structures
---
```
struct list
```

### Type Definitions
---
```
typedef struct list List
```

### Code Source
---
```
#ifndef _LIST_H_
#define _LIST_H_
#include <stdio.h>
#include <stdlib.h>
 
struct list
{
  struct list *next;
  int data;
};
 
// Initialize the sentinel of an empty list.
void list_init(struct list *list);
 
// Return true if the list is empty.
// Otherwise, return false.
// Do not forget that there is always a sentinel.
// So the list is empty if the sentinel does not point to a next element.
int list_is_empty(struct list *list);
 
// Return the length of the list (sentinel excluded).
size_t list_len(struct list *list);
 
// Insert 'elm' in front of the list, that is just after the sentinel.
// Note that 'elm' is already an existing element.
// You just have to insert it.
void list_push_front(struct list *list, struct list *elm);
 
// Extract the first element (not the sentinel) of the list.
// This operation removes the element from the list and returns it
// (the caller is responsible for freeing it).
// If the list is empty, the function returns NULL.
struct list* list_pop_front(struct list *list);
 
// Search for the first element that contains 'value' and return it
// (without removing it from the list).
// The function returns NULL if the value is not in the list.
struct list* list_find(struct list *list, int value);
 
// Return true if the list is sorted in increasing order.
// Otherwise, return false.
int list_is_sorted(struct list *list);
 
// Insert 'elm' in the sorted list (keeping the list sorted).
// Note that 'elm' is already an existing element.
// You just have to insert it.
void list_insert(struct list *list, struct list *elm);
 
// Reverse the elements of the list (except for the sentinel).
void list_rev(struct list *list);
 
#endif
```

### Function Documentation
---
#### ◆ list_find()
```
// Trouve un élément dans la liste chainée
// Prend en paramètre un pointeur sur la liste et la valeur à trouver
// Retourne un pointeur sur l'élément trouvé ou NULL
>> struct list* list_find (struct list * list, int value)
```

#### ◆ list_init()
```
// Initialise la liste chainée
// Prend en paramètre un pointeur sur la liste
// Ne retourne rien
>> void list_init (struct list * list)
```

#### ◆ list_insert()
```
// Insérer un élément dans la liste
// Prend en paramètre un pointeur sur la liste et un pointeur sur l'élément à insérer
// Ne retourne rien
>> void list_insert (struct list * list, struct list * elm)
```

#### ◆ list_is_empty()
```
// Vérifier si la liste est vide
// Prend en paramètre un pointeur sur la liste
// Retourne 1 si la liste est vide, 0 sinon
>> int list_is_empty (struct list * list)
```

#### ◆ list_is_sorted()
```
// Vérifier si la liste est triée
// Prend en paramètre un pointeur sur la liste
// Retourne 1 si la liste est triée, 0 sinon
>> int list_is_sorted (struct list * list)
```

#### ◆ list_len()
```
// Calculer la longueur de la liste
// Prend en paramètre un pointeur sur la liste
// Retourne la longueur de la liste
>> size_t list_len (struct list * list)
```

#### ◆ list_pop_front()
```
// Supprimer un élément au début de la liste
// Prend en paramètre un pointeur sur la liste
// Retourne un pointeur sur l'élément supprimé
>> struct list* list_pop_front (struct list * list)
```

#### ◆ list_push_front()
```
// Ajouter un élément au début de la liste
// Prend en paramètre un pointeur sur la liste et un pointeur sur l'élément à ajouter
// Ne retourne rien
>> void list_push_front (struct list * list, struct list * elm)
```

#### ◆ list_rev()
```
// Inverser la liste
// Prend en paramètre un pointeur sur la liste
// Ne retourne rien
>> void list_rev (struct list * list)
```
