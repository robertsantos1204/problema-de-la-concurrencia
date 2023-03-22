# problema de la concurrencia: semaforos 

##**robert santos 2021-0956**

- Concepto básico de semáforo en los sistemas operativos: 
son herramientas que provee el sistma operativo ,es una variable que solo se pueden acceder por medio de dos operaciones :wait y signal,wait para esperar y signal para dar acceso, Se inicializa a un valor no negativo (número máximo de procesos que podrán acceder a él sin bloquearse). Si un proceso ejecuta la operación wait sobre un semáforo, decrementa su valor. Si el valor resulta negativo, el proceso se bloquea.

- Explica en qué consisten los semáforos binarios y enteros:
Binarios: solo pueden tener dos valores 0 y 1
original o entero: puede tener muchos valores siempre y cuanto sean positivos 

- Explica la relacion entre los semáforos y la sincronizacio
Los semáforos constituyen un proceso de sincronización de procesos mas que de comunicación de información. Con ellos se pueden resolver problemas de exclusión mutua, en los que un recurso es compartido por varios procesos.
El wait y el signal son indivisibles y no se pueden interrumpir, es decir, no se pueden ejecutar ambas a la vez.
Los semáforos binarios los utilizaremos para recursos de una sola instancia, y para sincronización binaria.
