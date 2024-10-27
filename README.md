# AnalizadorSemantico
Creación de un análizador semántico


# Tarea Semana 5

Leer Capítulo 5 del Libro Compiladores, Principios, Técnicas y exponer en clases

# Ejercicios:

1)    Crear un analizador semántico de un compilador. (Utilizar cualquier herramienta) en el Lenguaje de programación de su preferencia.

2)    Subir el código a Github y enviar el código fuente y el ejecutable del proyecto a nube.utesa


# Detecciones actuales del Analizador Semántico
- Si se declara una variable fuera de main.
- Si se declara una variable más de una vez en el mismo ambito.
- Si se le añade un tipo de dato que no le corresponde a una variable (solo funciona int, float o double).
- Si una variable no ha sido declarada.



# Código para prueba
int main() {  
  int a = 0;  
  int i = 0.5; // debe dar error porque es entero  
  float p = 0.5;  
  int d = 0;  
  int d=0; //debe dar error porque ya fue declarada  
  
  for (a = 0; a < 3; a++) {  
    i++;  
    d = i;  
  }  
  d=0.5; // debe dar error porque es entera  
  
}  
