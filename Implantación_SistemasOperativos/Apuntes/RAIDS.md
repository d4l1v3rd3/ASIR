# RAID 0

Consiste en una serie de unidades de disco conectados en paralelo que permiten una transferencia sumltánea de datos a todos ellos, se obtiene gran velocdad de lectura y escritura.

![image](https://github.com/user-attachments/assets/eaadc5c2-2ebd-4d48-b6cb-c2caddfcbc1f)

Cada fichero se va guardando de forma aleatoria, si se rompe un disco se pierde información de dicho disco.

Utilizado: Para empresas de alto rendimiento de acceso a la información (videojuegos, animación)

# RAID 1

Alternativa costosa para grandes sistenas, unidades se han de añadir en pares para aumentar almacenaje.

![image](https://github.com/user-attachments/assets/8455f093-ccc7-4950-9e67-f93c00692fbe)

# RAID 5

Más eficaz y el de uso preferente en todos lugares. Mejor relación rendimiento-tolerancia-coste.

Es cada disco se genera una paridad, pudiendose reconstruir el disco estropeado.

Con la combinación de fraccionamiento de datos y paridad como método para recuperar datos en caso de error.

![image](https://github.com/user-attachments/assets/ae8f807c-0796-41bd-a2da-960f1f05600b)

# RAID 6

Elevado nivel de seguridad tiene como contrapartida un menor de rendimiento de escritua (Tenemos que hacer doble paridad) de cada dato.

No se comercializa dado que su coste es mucho mayor (controles requeridos que soporten doble paridad)

# RAID 10

Raid híbrido, RAID 1 + 0 combina las dos ventajas

![image](https://github.com/user-attachments/assets/9acdde10-9139-4217-acad-c29f8dfd986b)

Es el más rapido, el más seguro, pero el más costoso.

