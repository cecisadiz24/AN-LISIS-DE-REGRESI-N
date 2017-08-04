# practica1
a <- 4
b <-3
a+b 
suma <- a+b
#operaciones de comparación
a > b #a es mayor que b?
a <= a #a es igual mayor igual que 
a < b #a es menor que b?
a <= b
a == b #igualdad 
a!= b #a es diferente a b?

#COncepyo de función 

x<- abs(-2.5)##abs es la función del valotr absoluto 
x
help(abs)#pedir ayuda en R
x

#para asignar valores a variables en E se una <-
x<-"hola"###variable tipo caracter 
z<- 6 # el iguysl dolo funciona en una sola direccion
#utilizaremos objetos carcter y numerico 
ciudad <- "toluca"# una entrada
nombres <- c("karla", "rodrigo","miguel","Samuel") #caracter y 4 entradas 
edad <- c(28, 17,49,31)#numerico y 4 entradas 
##se utiliza la funcion class para preguntar a R que tipo de variable es 
class(nombres)
class(edad)

base1 <- data.frame(nombres,edad)#primer argumento filas 2 argumento columnas
View (base1)

ls(base1) # ver la lista de variables de la base 1 por ORDEN ALFABETICO

base1$edad #para mostrar los elemntos de una variable de la bse 

#### EJERCICIO Crear una variable de nombre sexo cpn 4 entradas 
#donde hombre es 1 y mujer es el valor 2, la primera entrada 
## es mujer y las otras tres hombres 
## despues de crear esta variable generen una nueva base 
#" de nombre base y cpom 3 variables nombre edad y sexo 
sexo<- c("2","1","1","1")
base2 <- data.frame(nombres,edad,sexo)
table(base2$sexo)
table(base2$edad)
#graficas
palumnos <- c(40,120,60,80)# alumnos fac economia 
etiq<- c("ACT","ECO","REI","NIB")
pie(palumnos)
pie(palumnos,etiq)

pie(palumnos,etiq,main=
      "grafica de pie de facultad de economia",
    sub="Fuentes:analisis de regresión",
    col= C("pink","blue","yellow","red"),
    radius=1.2, clockwise=TRUE, lTY=18)
