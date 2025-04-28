# Cancelar cupom via banco:

> _Ao realizar este processo as funções **128/** e **129/** para salvar e puxar cupom salvo **não valerão** para este cupom cancelado via banco._

-   Para ver o que tem no campo:  
    ```sql
    select STACUP, STACUPVRF from caixa;
    ```
-   Para alterar os campo para F:  
    ```sql
    update CAIXA set STACUP='F', STACUPVRF ='F';
    ```

