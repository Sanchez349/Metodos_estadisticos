# Metodos_estadisticos
## Licenciatura en Ingeniería Forestal

Curso de estadística de tercer semestre agosto diciembre 2026

Contenido De El Semestre 
**12/08/2026:Inicio de el Curso de métodos de estadísticos** 
*Preparar mi área de trabajo
*Crear una cuenta GITHUB "Sanchez349"
*Crear mi primer repositorio
*Modificar el archivo _README_
fecha 
sanchez
13/08/26


#Datos sin valor extremo
x1 <- c(1.2,1.5,1.7,1.8)
summary(x1)
mean(x1)
median(x1)
var(x1)
sd(x1)

# Datos con valor extremo 
x2 <- c(1.2,1.5,1.7,1.8,4.8)
summary(x2)
mean(x2)
median(x2)
var(x2)
sd(x2)

anillos <- data.frame(
  Arbol = 1:40,
  RW = c(1.42, 1.58, 1.71, 1.63, 1.85, 1.94, 2.06, 1.76, 1.68, 1.89, 2.14, 1.53, 1.79, 1.97, 2.23, 1.61, 1.82, 2.08, 1.73, 1.87, 1.91, 2.04, 1.76, 1.83, 2.12, 1.69, 1.57, 1.88, 2.21, 1.95, 1.74, 1.81, 2.09, 1.66, 1.92, 2.17, 1.72, 1.86, 2.02, 3.48)
)
#Media
mean(anillos$RW)
#mediana
median(anillos$RW)
#valor minimo
min(anillos$RW)
#valor maximo 
max(anillos$RW)
#Desviacion estandar 
sd(anillos$RW)
#varianza
var(anillos$RW)
#rango
max(anillos$RW)-min(anillos$RW)
#coeficiente de variacion 
(sd(anillos$RW)/mean(anillos$RW))*100

boxplot.stats(anillos$RW)$out