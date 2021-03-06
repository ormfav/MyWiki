# Funzioni Generatrici {#Funzioni Generatrici}

-   []{#T}**T** : Un mapping $f:(p,1)->(P,Q)$ è simplettico iff esiste
    localmente S(q,p) tc $P^T dQ - p^T dq = dS$
    1.  Scrivo Jf a blocchi ($P_p,P_q//Q_p,Q_q$)
    2.  Inserisco nella \[condizione di
        simpletticità\](trasformazioni-simplettiche.md) e moltiplico
    3.  simpletticità iff $P_p^T Q_p=Q_p^T P_p$,
        $P_p^T Q_q-id=Q_p^T P_q$, $Q_q^T P_q = P_q^T Q_q$
    4.  sviluppo $dQ(p,q)$ e inserisco in eq di tesi. Eguaglio eq di
        tesi
    5.  Ottengo $F(P,Q)(dp,dq)^T$
    6.  Calcolo JF
    7.  Per \[lemma di integrabilità\](trasformazioni-simplettiche.md) f
        è grad di S se Jf è simmetrica
    8.  Simmetria di Jf coincide con le 3 eq di simpletticità trovate
-   Idea: teorema suggerisce di cambiare coordinate $z=(q,Q)$
    -   è possibile per \[Dini\] se $dQ/dp$ è invertibile
    -   $y=h(z)$
-   Se f è simplettico, può essere ottenuto da $S(q,Q)=S(h(z))$:
    $P=dS(q,Q)/dQ$, $p=-dS(q,Q)/dq$
    -   Basta sostituire nell\'eq del teorema, scrivere esplicitamente S
        e confrontare i coeff
-   []{#T}**T** : $f:(p,q)->(P,Q)$ vicina all\'identità è simplettica
    iff, per certe $S^1(P,q)$, $S^2(p,Q)$, $S^3((P+p)/2,(Q+q)/2)$
    -   $Q^TdP+p^Tdq=d(P^Tq+S^1)$
    -   $P^TdQ+q^Tdp=d(p^TQ-S^2)$
    -   $(Q-q)^Td(P+p)-(P-p)^Td(Q+q)=2dS^3$
        1.  Primo caso:
            1.  scelgo di cambiare coord $z=(P,q)$ e scelgo s(P,q) come
                funzione generatrice
            2.  osservo $P^T dQ=d(P^T Q)-Q^T dP$
            3.  Sostituisco nell\'eq del teorema ottenendo
                $Q^T dP+p^T dQ=d(P^T Q-S)$
            4.  Segue $s=P^T Q-S$
            5.  Prendo $S^1$ tc $s=P^T q+S^1$
        2.  Secondo caso:
            1.  scelgo coord $z=(p,Q)$ e s(p,Q) come funzione
                generatrice
            2.  osservo $p^T dq=d(p^T q)-q^T dp$
            3.  proseguo come nel primo caso
        3.  Terzo caso:
            1.  []{#-da-finire}[da-finire]{#da-finire .tag}
    -   Le S sono scelte tc si abbia id quando vengono sostituite con 0
