# Semana 3

**Álgebra de Boole**

*AND (Conjunción)*: La operación AND entre dos variables es verdadera (1) solo si ambas son verdaderas.

Ejemplo: A * B o A ∧ B

*OR (Disyunción)*: La operación OR entre dos variables es verdadera si al menos una de ellas es verdadera.

Ejemplo: A + B o A ∨ B

*NOT (Negación)*: La operación NOT invierte el valor de la variable. Si la variable es verdadera (1), se convierte en falsa (0), y viceversa.

Ejemplo: ¬A ó ~A (también puede encontrarse con la Ā)

Dentro del álgebra de Boole, es de utilidad definir que está compuesta por solo dos elementos. Es un conjunto de elementos binarios relacionados entre sí mediante las operaciones lógicas, producto (*) y suma (+), que cumplen con los siguientes postulados:

*ELEMENTO IDENTIDAD*

a + 0 = a

a * 1 = a

*PROPIEDAD CONMUTATIVA*

a + b = b + a

a * b = b * a

*PROPIEDAD DISTRIBUTIVA*

a * (b + c) = (a * b) + (a * c)

a + (b * c) = (a + b) * (a + c)

*INVERSIÓN LÓGICA (ó COMPLEMENTACIÓN)*

a + ¬a = 1

a * ¬a = 0 

***

**Teoremas**


1) Dualidad: toda igualdad lógica sigue siendo válida si se intercambian los operadores ( +  y * ) y los elementos de identidad (0 y 1). La simetría de los postulados demuestra este  teorema.

2)  El álgebra es un conjunto cerrado; es decir, los resultados de aplicar las operaciones lógicas a las variables, pertenecen al álgebra.

3) En el álgebra se cumple que

         a + 1 = 1
         a * 0 = 0

4) Ley de Idempotencia

         a + a = a
         a * a = a

5) Ley de involución
 
         (a’)’ = a

6) Las operaciones lógicas son asociativas

         a + (b + c) = (a + b) + c
         a . (b . c) = (a . b) . c

7) Absorción:
 
         a = a + (a . b)
         a = a . (a + b)
         a + (¬a * b) = (a + b)
         a * (¬a + b) = (a * b)

8) Leyes de De Morgan

         (a + b + c + d + .......+ n)’ = a’ . b’ . c’ . d’ ...........n’
         (a . b . c . d .........n)’ = a’ + b’ + c’ + d’ + ..........+ n’

9) Asociativa

       a- Con respecto a la disyunción

                       ((a + b) + c) = (a + (b + c))
         
       b- Con respecto a la conjunción
                       
                       ((a * b) + c) = ((a + c) * (b + c))

10) Conmutativa

     a- Con respecto a la disyunción

                       (a + b)  = (b + a)
         
     b- Con respecto a la conjunción
                       
                       (a * b)  = (b * a)
11) Distributiva

     a- De la conjunción respecto a la disyunción

                      [(a + b) * c] = [(a * c) + (c * b)]

     b- De la disyunción respecto a la conjunción

                      [(a * b) + c] = [(a * c) + (b * c)]

12) Condicional 

     a → b = ¬a + b

13) Negación de la Condicional 

     ¬(a → b) = a * ¬b

14) Condicional contrarrecíproca

     a → b = ¬a → ¬b

15) Transportación

      (a → b) * (b → c) = a → c

***

*Suma booleana* 

* 0 + 0 = 0
* 0 + 1 = 1
* 1 + 0 = 1
* 1 + 1 = 1

*Multiplicacion booleana*

* 0 * 0 = 0
* 0 * 1 = 0
* 1 * 0 = 0
* 1 * 1 = 1

***

*Reglas basicas y simplificacion logica*

1. A  + 0 = A

Si aplicamos la operación OR a una variable cualquiera y a 0, el resultado es siempre igual a la variable.  Si A es 1, la salida es igual a 1 y, por tanto, igual a A.  Si A es 0, la salida es 0, e igualmente, es idéntica a A.

2. A + 1 = 1

Si se aplica la operación OR a una variable y a 1, el resultado es siempre igual a 1.  Un 1 en una entrada de una puerta OR produce siempre un 1 en la salida, independientemente del valor de la otra entrada.

3. A * 0 = 0

Si se aplica la operación AND a una variable y a 0, el resultado es siempre igual a 0.  Siempre que una de las entradas de una puerta AND sea 0, la salida es siempre 0, independientemente del valor de la otra salida. 

4. A * 1 = A

Si aplica la operación AND a una variable y a 1, el resultado es siempre igual a la variable.  Si la variable A es 0, la salida de la puerta AND será siempre 0, mientras que si A es 1, la salida será 1, dado que las dos entradas son 1.

5. A + A = A

Si se aplica la operación OR a una variable consigo misma, el resultado es siempre igual a la variable.  Si A es 0, entonces 0 + 0 = 0, mientras que si A es 1, 1 + 1 = 1.

6. A + ¬A = 1

Si se aplica la operación OR a una variable y a su complemento, el resultado es siempre igual a 1.  Si A es 0, entonces 0 + ¬0 = 0 + 1 = 1.  Si A es 1, entonces 1 + ¬1 = 1 + 0 = 1.

7. A * A = A

Si se aplica la operación AND a una variable consigo misma, el resultado siempre es igual a la variable.  Si A = 0, entonces 0 * 0 = 0, y si A = 1, entonces 1 * 1 = 1.

8. A * ¬A = 0

Si se aplica la operación AND a una variable y a su complemento, el resultado es siempre igual a 0.  Esta regla se basa en que siempre A o ¬A será 0, y además en que cuando se aplica un 0 a una de las entradas de una puerta AND, la salida siempre es 0.

9. ¬(¬A) = A

El complemento del complemento de una variable es siempre la propia variable.  El complemento de la variable A es ¬A y el complemento de ¬A será de nuevo A, que es la variable original.

10. A + AB = A 

A esta regla se la puede obtener aplicando la ley distributiva y las reglas 2 y 4, de la siguiente manera: 

A + AB = A(1 + B)     sacar factor común (ley distributiva)

            = A * 1           regla 2: (1 + B) = 1

            = A                regla 4: A * 1 = A

11. A + ¬AB = A + B

Esta regla puede demostrarse de la siguiente manera:

A + ¬AB = (A + AB) + ¬AB              regla 10: A = A + AB

              = (AA + AB) + ¬AB            regla 7: A = AA

              = AA + AB + A¬A + ¬AB    regla 8: sumar A¬A=0

              = (A + ¬A) (A + B)              sacar factor común

              = 1 * ( A + B)                      regla 6: A + ¬A = 1

              = A + B                               regla 4: eliminar el 1 

12. (A + B) * (A + C) = A + BC

Esta regla puede demostrarse de la siguiente manera:

( A + B ) * ( A + C ) = AA + AC + AB + BC    Ley distributiva

                              =  A + AC + AB + BC     regla 7: AA = A

                              =  A (1 + C) + AB + BC  sacar factor común (Ley distributiva)

                              =  A * 1 + AB + BC         regla 2: 1 + C = 1

                              = A (1 + B) + BC            sacar factor común (Ley distributiva)

                              =  A * 1 + BC                  regla 2: 1 + B = 1

                               = A + BC                        regla 4: A * 1 = A
