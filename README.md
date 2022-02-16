algoritmo "analisador_de_valores"

var
    c,v,totv,n,vp,d5:inteiro

inicio  
    c<-1
    para c:=1 ate 5 faca
        escreva("Digite o",c, "º. valor: ")
        leia(v)
    totv<-totv+v
    c<-c+1
        se v=0 entao
            n<-n+1
        senao
            se  v%2=0 entao
                vp<-vp+v
                senao
                se v%5=0 entao
                    d5<-d5+1
                    fimse
                fimse
            fimse
    fimpara

    escreval("A soma entre os valores é ",totv)
    escreval("A média entre os valorea é ",totv/5)
    escreval("Valores divisíveis por 5: ",d5)
    escreval("Valores nulos: ",n)
    escreval("A soma dos valores pares é: ",vp)
    fimalgoritmo
