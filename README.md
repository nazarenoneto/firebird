

Exemplos:

1) Para obter o valor futuro de uma operação
<pre>     n = 10
     i = 2%
     pv = 1000
     fv = ?
     
     select  PKG_FINANCE.fv(1000,2,10) FV from rdb$database                  (3.0)
        ou
     select  * from fin_fv(1000,2,10)                                        (2.5)
     
     Resposta: 1218.994 </pre>     
     
2) Para obter o valor presente de um valor futuro
<pre>
   n = 10
   i = 2%
   fv = 1218,994
   pv = ?
   
   select  PKG_FINANCE.pv (1218.994,2,10) PV from rdb$database          (3.0)
      ou
   select * from fin_pv (1218.994,2,10)                                 (2.5) 
   
   Resposta:  1000.00</pre>
   
3) Para obter o valor de uma prestação em um financiamento de parcelas uniformes
<pre>
   pv = 1000
   n = 10
   i = 2%
   pmt = ?
   
   select  PKG_FINANCE.pmt (1000,2,10) pbm from rdb$database   (3.0)
        ou
   select  * from fin_pmt(1000,2,10)                           (2.5)
   
   Resposta: 111.33</pre>


   
   
   
   
   
   
     
