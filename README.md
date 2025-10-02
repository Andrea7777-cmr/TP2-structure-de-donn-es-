# TP2-structure-de-donn-es-
#include <stdio.h> 
#include <stdlib.h>

struct Cellule{
    int a;
    struct Cellule *suiv;
};
typedef struct Cellule *liste;
liste L;
voidmain(int nbOccurence; elmt *rechercerElmt(elmt *liste,int b)){
        elmt *tempo=liste;
        while(tempo!=NULL){
            if(tempo->==b)
            printf("afficher %d" b);
            int supprimerOccurences(elmt *liste,int b){
                while(nbOccurence!=NULL)
                free(courant);
            }
            else 
            printf("l'element n'existe pas");
        }    
        return 0;

    }

2---------------------------------------------------------------------------------------------------------------------------------------------
int comparer(liste L,int *a,int *b) {
    return (tri((int*)a - *(int*)b)); // Tri croissant
}
    // Insertion en debut de liste
 void Insertiontete(struct Cellule *L ,int b){
    scanf("%d" n);
    L<- NULL;
    i<- 1;
    do{
        scanf("%d" b);
        L=  malloc(sizeof(cellule));
        L<- info= b;
        L<- suiv= suiv;
        L<- L;
        i++;
        while(i==n+1)
    }
    return 0;
}    
    //Insertion en fin de liste
voi insertionfin(struct Cellule *L, int b){
    Cellule *P= (Cellule*)malloc(sizeof(Cellule));
    P->a = b;
    P->suiv = NULL;

    if(*L == NULL){
        *P = L;
    }
    else{
        Cellule *temp = *L;
        while (temp->suiv != NULL){
            temp = temp-> = suiv;
        }
        temp->suiv = P;
    }
}
3------------------------------------------------------------------------------------------------------------------------------------
// Définition d'un nœud de la liste doublement chaînée
typedef struct Cellule {
    int value;
    struct Cellule* prec;
    struct Cellule* suiv;
} Cellule;
Cellule *Liste;
Liste l;

// Création d’un nouveau nœud
Cellule* creerCellule(int value) {
    Cellule* L = (Cellule*)malloc(sizeof(Cellule));
    L->value = value;
    L->prec = NULL;
    L->suiv = NULL;
    return L;
}

// Insertion en début de liste
void Insertiontete(Cellule** l, int value) {
    Cellule* L = creerCellule(value);
    L->suiv = *l;
    if (*l != NULL) {
        (*l)->prec = L;
    }
    *l = L;
}

// Insertion à la fin de la liste
void insertionfin(Cellule** l, int value) {
    Cellule* L = creerCellule(value);
    if (*l == NULL) {
        *l = L;
        return (Insertiontete(l,value));
    }
    Cellule* temp = *l;
    while (temp->suiv != NULL) {
        temp = temp->suiv;
    }
    temp->suiv = L;
    L->prec = temp;
}
4-----------------------------------------------------------------------------------------------------------------------
// Insertion dans une position quelconque
void insertionliste(Cellule* precedent, int value) {
    if (precedent == NULL) {
        printf("Le nœud précédent ne peut pas être NULL\n");
        return 1;
    }
    Cellule* L = creerCellule(value);
    L->suiv = precedent->suiv;
    precedent->suiv = L;
    L->prec = precedent;

    if (L->suiv != NULL) {
        L->suiv->prec = L;
    }
}

// Définition de la structure
typedef struct Cellule {
    int val;
    struct Cellule *suiv;
} Cellule;
Cellule *Liste;
Liste L;

// Insertion en tête
void Insertiontete(Cellule **L, int b) {
    Cellule *P = (Cellule *)malloc(sizeof(Cellule));
    P->val = b;

    if (*L == NULL) {
        // Premier élément pointe sur lui-même
        P->suiv = P;
        *L = P;
    } 
    else {
        Cellule *temp = *L;
        while (temp->suiv != *L)
            temp = temp->suiv;

        P->suiv = *L;
        temp->suiv = P;
        *L = P;
    }
    return 0;
}

// Insertion en queue
void insertionqueue(Cellule **L, int b) {
    Cellule *P = (Cellule *)malloc(sizeof(Cellule));
    P->val = b;

    if (*L == NULL) {
        P->suiv = P;
        *L = P;
    }
     else {
        Cellule *temp = *L;
        while (temp->suiv != *L)
            temp = temp->suiv;
        temp->suiv = P;
        P->suiv = *L;
    }
    return 0;
}
5--------------------------------------------------------------------------------------------------------------------------------------
// Définition de la structure
typedef struct Cellule {
    int val;
    struct Cellule *suiv;
    struct Cellule *prec;
} Cellule;
Cellule *Liste;
Liste L;

// Insertion en tête
void Insertiontete(Cellule **L, int b) {
    Cellule *P = (Cellule *)malloc(sizeof(Cellule));
    P->val = b;

    if (*L == NULL) {
        P->suiv = P;
        P->prec = P;
        *L = P;
    }
     else {
        Cellule *queue = (*L)->prec;

        P->suiv = *L;
        P->prec = queue;
        queue->suiv = P;
        (*L)->prec = P;
        *L = P;
    }
    return 0;
}

// Insertion en queue
void insertionqueue(Cellule **L, int b) {
    Cellule *P = (Cellule *)malloc(sizeof(Cellule));
    P->val = b;

    if (*L == NULL) {
        P->suiv = P;
        P->prec = P;
        *L = P;
    } 
    else {
        Cellule *queue = (*L)->prec;

        P->suiv = *L;
        P->prec = queue;
        queue->suiv = P;
        (*L)->prec = P;
    }
    return 0;
}




-------------
// Définition de la structure
typedef struct Cellule {
    int val;
    struct Cellule *suiv;
    struct Cellule *prec;
} Cellule;
Cellule *Liste;
Liste L;

// Insertion en tête
void Insertiontete(Cellule **L, int b) {
    Cellule *P = (Cellule *)malloc(sizeof(Cellule));
    P->val = b;

    if (*L == NULL) {
        P->suiv = P;
        P->prec = P;
        *L = P;
    }
     else {
        Cellule *queue = (*L)->prec;

        P->suiv = *L;
        P->prec = queue;
        queue->suiv = P;
        (*L)->prec = P;
        *L = P;
    }
    return 0;
}

// Insertion en queue
void insertionqueue(Cellule **L, int b) {
    Cellule *P = (Cellule *)malloc(sizeof(Cellule));
    P->val = b;

    if (*L == NULL) {
        P->suiv = P;
        P->prec = P;
        *L = P;
    } 
