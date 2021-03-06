# Sistemi Integrabili {#Sistemi Integrabili}

-   domanda: Sotto quali condizioni un sistema hamiltoniano (dimensione
    2n) è integrabile?
-   idea: cerchiamo [trasformazione
    canonica](funzioni-generatrici.wiki "wikilink") $(p,q)->(x,y)$ che
    semplifichi il sistema
    -   ovvero $H(p,q)=K(x)$ in modo che il sistema diventi $dx/dt=0$,
        $dy/dt=w(x)$
        -   il sistema è integrabile: $x(t)=cost$, $y(t)=w(x)t+c$
    -   significa richiedere che la funzione generatrice soddisfi eq
        differenziale $H(dS/dq,q)=K(x)$ (eq di Hamilton-Jacobi)
    -   gli $x_i=F_i(p,q)$ sono integrali primi del moto in involuzione
-   []{#T}**T**: Se ho n funzioni $F_i$ in involuzione fra loro in un
    intorno di $(q_0,p_0)$ e i loro gradienti sono l.i. in $(q_0,p_0)$
    allora esistono n funzioni lisce $G_i$ definnite in un intorno di
    $(q_0,p_0)$ che completano la trasformazione
    $(p,q)->(F_1...F_n,G_1...G_n)=(x,y)$
    1.  Siccome i gradienti delle $F_i$ sono l.i. n colonne della
        matrice nx2n JF sono l.i.
    2.  Dopo trasformazioni canoniche di permutazione delle coordinate
        ottengo una sottomatrice nxn invertibile, ad es $F_p=dF/dp$
    3.  \[Dini\] mi dice che $x=F(p,q)$ può essere localmente risolta
        per p, ovvero $p=P(x,q)$, $P_x=F_p^{-1}$, $P_q=-F_p^{-1}F_q$
    4.  ${F_i,F_j}=0 => F_pF_q^T-F_qF_p^T=0$
    5.  Moltiplico a destra per $F_p^{-T}$ e a sinistra per $F_p^{-1}$
        ottenendo $-P_q^T+P_q=0$ ovvero $P_q$ è simmetrica
    6.  Per \[lemma di integrabilità\](trasformazioni-simplettiche.md)
        P(x,q) è localmente il gradiente rispetto alle q di S(x,q)
    7.  $d^2S/dxdq=P_x=F_p^{-1}$ è invertibile dunque $y=dS/dx=G$,
        $p=dS/dq$ è trasformazione simplettica (x=F per costruzione)
    8.  Se le $F_i$ sono integrali del moto posso costruire il sistema
        semplificato, in quanto $H(p,q)=F_1(p,q)=x_1=K(x)$
-   problema: lemma locale, non mi dice nulla sulla dinamica del sistema
-   []{#D}**D** : Un sistema con hamiltoniana $H:McR^{2n}->R$ è detto
    completamente integrabile se esistono n funzioni lisce $F_i$ (con
    $F_1=H$) tali che
    1.  $F_i$ sono i involuzione
    2.  i loro gradienti sono l.i. in ogni punto di M (passaggio da
        locale di lemma a globale)
    3.  esistono per ogni t le traiettorie dei sistemi con hamiltoniane
        $F_i$ e queste traiettorie stanno in M
-   noto che:
    -   ora tutti i sistemi $F_i$ sono completamente integrabili
        ($F_1=H$ non riveste un ruolo speciale)
    -   Quindi per il punto 1 tutti gli $F_j$ sono integrali del sistema
        con Hamiltoniana $F_i$
    -   I flussi di ciascuna di queste Hamiltoniane commutano \[lemma
        lubich pag 279\]
-   Introduciamo l\'insieme di livello $M_x={(p,q)cM|F(p,q)=x}$
-   []{#T}**T** : $F_i: M->R$ soddisfano la definizione, $M_x$ non vuoto
    e connesso in un intorno di $x_0\in R^n$ allora in B intorno di
    $x_0$ esiste un mapping simplettico e suriettivo
    $e:BxR^n -> U_{x\in B} M_x, (x,y) -> (p,q)$ che linearizza i flussi
    dei sistemi con Hamiltoniane $F_i$, ovvero $f_t^i(p,q)=e(x,y+te_i)$
    (e_i versore)
    1.  Chiamo $l: (p,q)->(x,y)$ la trasformazione del teorema
        precedente in un intorno U di $(x_0,y_0)$, con
        $l(p_0,q_0)=(x_0,y_0)$
    2.  a v in $R^n$ associo l\'Hamiltoniana $F_v=v_iF_i$ (somma
        einstein)
    3.  Siccome ${F_i,F_j}=0$ i loro flussi commutano e dunque
        $f_{tv}=f_{tv_1}^1...f_{tv_n}^n$
    4.  l trasforma il sistema con Hamiltoniana $F_v$ in
        $dx/dt=0,dy/dt=v$
    5.  Il seguente schema commuta per (p,q) in U e tv piccoli
                        (p,q) ----> f_{vt}(p,q)
                          | ............ ^
                          | ............ |
                          l .......... l^{-1}
                          | ............ |
                          v ............ |
                        (x,y) ------> (x,y+tv)
    6.  Costruiamo $e: (x,y)->(x,y_0)->(p,q)->f_y(p,q)$,
        $e(x,y)=f_y(l^{-1}(x,y_0))$ 7.
        -   e è simplettico in quanto composizione di trasformazioni
            simplettiche
        -   Per come è stato definito, chiaramente vale
            $f_t^i(p,q)=e(x,y+te_i)$
        -   $M_x$ è invariante sotto $f_t^i$ e $l^{-1}(x,y_0)$ è in
            $M_x$ dunque e(x,y) è in $M_x$ per ogni (x,y)
    7.  Resta da mostrare suriettività \...
-   []{#T}**T** (arnol\'d -liouville) : F come da definizione, $M_x$
    compatto e connesso per ogni x in un intorno di $x_0$ in $R^n$.
    Allora esistono intorni B di $x_0$ e D di 0 tali che: per ogni x M_x
    sia $T^n$ invariante sotto il flusso dei sistemi con Hamiltoniana
    $F_i$; esiste una trasformazione simplettica biiettiva
    $\psi: DxT^d -> U_{x\in B} M_x c R^nxR^n, (a,\theta)->(pq)$ tc
    $F_i(\psi(a,theta))=f_i(a)$ con $f_i:D->R$ -$(a,\theta)$ sono dette
    variabili azione-angolo
    1.  \[dimostrazione arnold liouville\]
