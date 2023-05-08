# table.c File Reference
---
```
#include <tree.h>
```

## Functions
---
```
struct tree * createTree (int data)
size_t tree_size (struct tree *t)
size_t max (size_t a, size_t b)
size_t tree_height (struct tree *t)
void free_tree (struct tree *t)
struct tree * ajouter_noeud (struct tree *racine, int valeur)
struct tree * minimum_dans_sous_arbre_droit (struct tree *racine)
struct tree * supprimer_noeud (struct tree *racine, int valeur)
void prefix_print (struct tree *t)
void infix_print (struct tree *t)
```

## Function Documentation
---
### ◆ ajouter_noeud()
```
>> struct tree* ajouter_noeud (struct tree * racine, int valeur)
```

### ◆ createTree()
```
>> struct tree* createTree (int data)
```

### ◆ free_tree()
```
>> void free_tree (struct tree * t)
```

### ◆ infix_print()
```
>> void infix_print (struct tree * t)
```

### ◆ max()
```
>> size_t max (size_t a, size_t b)
```

### ◆ minimum_dans_sous_arbre_droit()
```
>> struct tree* minimum_dans_sous_arbre_droit (struct tree * racine)
```

### ◆ prefix_print()
```
>> void prefix_print (struct tree * t)
```

### ◆ supprimer_noeud()
```
>> struct tree* supprimer_noeud (struct tree * racine, int valeur)
```

### ◆ tree_height()
```
>> size_t tree_height (struct tree * t)
```

### ◆ tree_size()
```
>> size_t tree_size (struct tree * t)
```
