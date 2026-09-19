# Operadores e Estrutura de Fluxo em Javascript

* Operadores: 
   * Operadores Aritméticos: 
      * Soma (`+`);
      * Subtração (`-`);
      * Multiplicação (`*`);
      * Potência (`**`);
      * Divisão (`/`);
      * Resto (`%`).

   * Operadores de atribuição:
      * `valor = 5;`;
      * `valor += 5;`;
      * `valor -= 5;`;
      * `valor++;`;
      * `valor--;`.

   * Operadores Relacionais:
      * `1 === 5` (`false`);
      * `10 !== "10"` (`true`);
      * `"1" == 1` (`true`);
      * `"15" != 15` (`false`);

      ---
      
      * `10 > 5` (`true`);
      * `3 < 3` (`false`);
      * `12 <= 12` (`true`);
      * `5 >= 6` (`false`).

   * Operadores Lógicos:
      * `true && false` (Operador `AND`, resultado: `false`);
      * `true || false` (Operador `OR`, resultado: `true`);
      * `!false` (Operador `NOT`, resultado: `true`).

   * Operador ternário:
      * `condição` ? `resultado caso verdadeiro` : `resultado caso falso`;

* Estruturas:
   * Estrutura condicionais:
      * if / else:
         ```js
         if (condicao1) {
            comando1; // Realiza caso o primeiro seja verdadeiro
         } else if (condicao2) {
            comando2; // Realiza caso o primeiro seja falso e segundo verdadeiro
         } else {
            comando3; // Realiza caso todos o if forem falsos.
         }
         ```

      * switch case:
         ```js
         switch (valor) {
            case 1:
               comando1; // valor sendo 1
               break;
            case 2:
               comando2; // valor sendo 2
               break;
            case 3:
            case 4:
               comando3; // valor sendo 3 ou 4
               break;
            default:
               comando4; // valor não sendo nenhum esperado.
         }
         ```
   
   * Estrutura condicionais:
      * for:
         ```js
         // for (inicialização; condição de parada; incremento)
         for (let k = 1; k <= 10; k++) {
            console.log(k); // 1, 2, 3, 4, 5, 6, 7, 8, 9, 10.
         }

         for (let i = 0, j = 10; i <= j; i++, j--) {
            console.log(i+j); // 10, 10, 10, 10, 10, 10.
         }
         ```

      * while:
         ```js
         let fibo0 = 0, fibo1 = 1, fibo2 = 1;

         while (fibo2 < 100) {
            fibo2 = fibo1 + fibo0;
            fibo0 = fibo1;
            fibo1 = fibo2;
         }
      
         console.log(fibo2); // 89
         ```

      * do-while:
         ```js
         let aleatorio = Math.floor(Math.random() * 100) + 1;

         do {
            let num = Number(prompt("Informe um numero de 1 a 100: "));
         } while (num !== aleatorio);
         ```
