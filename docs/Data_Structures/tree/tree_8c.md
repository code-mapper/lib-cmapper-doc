## Documentation Arbres
---
```
#include <tree.h>
```

### Qu'est ce qu'un arbre ?
Un arbre est une structure de données non linéaire qui permet de stocker des éléments de façon hiérarchique. Un arbre est composé d'un noeud racine et de sous-arbres. Chaque sous-arbre est lui-même un arbre. Un arbre est composé de noeuds. Chaque noeud est composé d'une valeur et de deux pointeurs vers les sous-arbres gauche et droit.

###  Definition d'un arbre
---
```
int value
struct tree * left
struct tree * right
```

###  Documentation des attributs
---
#### ◆ left
```	
>> struct tree * left
```
#### ◆ right
```
>> struct tree * right
```

#### ◆ value 
```
>> int value
```

### Data Structures
---
```
struct tree
```

### Type Definitions
---
```
typedef struct tree Tree
```

### Code Source
---
```
#ifndef TREE_H_
#define TREE_H_
 
 
#include <stdlib.h>
#include <stdio.h>
 
 
struct tree
{
    int value;
    struct tree* left;
    struct tree* right;
};
 
struct tree* createTree(int data);
size_t tree_size (struct tree* t);
size_t max (size_t a, size_t b);
size_t tree_height (struct tree* t);
void free_tree (struct tree* t);
struct tree* ajouter_noeud(struct tree* racine, int valeur);
struct tree* supprimer_noeud(struct tree* racine, int valeur);
void prefix_print(struct tree* t);
void infix_print(struct tree* t);
void prefix_print(struct tree* t);
#endif
```

### Documentation des fonctions
---
#### ◆ ajouter_noeud()
```
>> struct tree* ajouter_noeud (struct tree * racine, int valeur)
```

#### ◆ createTree()
```
>> struct tree* createTree (int data)
```

#### ◆ free_tree()
```
>> void free_tree (struct tree * t)
```

#### ◆ infix_print()
```
>> void infix_print (struct tree * t)
```

#### ◆ max()
```
>> size_t max (size_t a, size_t b)
```

#### ◆ minimum_dans_sous_arbre_droit()
```
>> struct tree* minimum_dans_sous_arbre_droit (struct tree * racine)
```

#### ◆ prefix_print()
```
>> void prefix_print (struct tree * t)
```

#### ◆ supprimer_noeud()
```
>> struct tree* supprimer_noeud (struct tree * racine, int valeur)
```

#### ◆ tree_height()
```
>> size_t tree_height (struct tree * t)
```

#### ◆ tree_size()
```
>> size_t tree_size (struct tree * t)
```

