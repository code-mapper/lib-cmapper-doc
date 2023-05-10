# linked_list.c File Reference
---
```
#include <stdlib.h>
#include "list.h"
```

<!-- ## Functions
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
-->

## Function Documentation
---
### ◆ list_find()
```
// Trouve un élément dans la liste chainée
// Prend en paramètre un pointeur sur la liste et la valeur à trouver
// Retourne un pointeur sur l'élément trouvé ou NULL
>> struct list* list_find (struct list * list, int value)
```

### ◆ list_init()
```
// Initialise la liste chainée
// Prend en paramètre un pointeur sur la liste
// Ne retourne rien
>> void list_init (struct list * list)
```

### ◆ list_insert()
```
// Insérer un élément dans la liste
// Prend en paramètre un pointeur sur la liste et un pointeur sur l'élément à insérer
// Ne retourne rien
>> void list_insert (struct list * list, struct list * elm)
```

### ◆ list_is_empty()
```
// Vérifier si la liste est vide
// Prend en paramètre un pointeur sur la liste
// Retourne 1 si la liste est vide, 0 sinon
>> int list_is_empty (struct list * list)
```

### ◆ list_is_sorted()
```
// Vérifier si la liste est triée
// Prend en paramètre un pointeur sur la liste
// Retourne 1 si la liste est triée, 0 sinon
>> int list_is_sorted (struct list * list)
```

### ◆ list_len()
```
// Calculer la longueur de la liste
// Prend en paramètre un pointeur sur la liste
// Retourne la longueur de la liste
>> size_t list_len (struct list * list)
```

### ◆ list_pop_front()
```
// Supprimer un élément au début de la liste
// Prend en paramètre un pointeur sur la liste
// Retourne un pointeur sur l'élément supprimé
>> struct list* list_pop_front (struct list * list)
```

### ◆ list_push_front()
```
// Ajouter un élément au début de la liste
// Prend en paramètre un pointeur sur la liste et un pointeur sur l'élément à ajouter
// Ne retourne rien
>> void list_push_front (struct list * list, struct list * elm)
```

### ◆ list_rev()
```
// Inverser la liste
// Prend en paramètre un pointeur sur la liste
// Ne retourne rien
>> void list_rev (struct list * list)
```
