

# python triple pitagoras

for  lado1  in  range(1, 501):

for  lado2  in  range(lado1, 501):

for  hipotenusa  in  range(lado2, 501):

if  lado1**2  +  lado2**2  ==  hipotenusa**2:

print("Lado1:", lado1, "Lado2:", lado2, "Hipotenusa:", hipotenusa)


# c++ triple pitagoras


/aplicacion para encontrar los triples de pitagoras menores a 500/
#include <iostream>
#include <cmath>
using namespace std;

int main() {
	cout << "Triples de Pitagoras menores a 500: \n";
    for (int a = 1; a <= 500; ++a) {
        for (int b = a; b <= 500; ++b) {
            for (int c = b; c <= 500; ++c) {
                if (a * a + b * b == c * c) {
                    cout << "Lado 1: " << a << ", Lado 2: " << b << ", Hipotenusa: " << c << "\n";
                }
            }

# Pseudocodigo triple de pitagoras

Algoritmo triplepitagorico
    Mostrar "Triples de Pitágoras:"
	Para a<-1 Hasta 500 Con Paso 1 Hacer
		Para b<-a Hasta 500 Con Paso 1 Hacer
			Para c<-b Hasta 500 Con Paso 1 Hacer
				Si a * a + b * b es igual a c * c Entonces
					Mostrar "Lado 1: ", a, ", Lado 2: ", b, ", Hipotenusa: ", c, " "
				Fin Si
				
			Fin Para
			
		Fin Para
	Fin Para

FinAlgoritmo
# python ahorcado


import  random

  

def  elegir_palabra():

palabras  = ["hola", "programacion", "ingenieria", "carro", "python", "desarrollador"]

return  random.choice(palabras)

  

def  mostrar_palabra(palabra, letras_adivinadas):

display  =  ""

for  letra  in  palabra:

if  letra  in  letras_adivinadas:

display  +=  letra

else:

display  +=  "_"

return  display

  

def  main():

palabra_a_adivinar  =  elegir_palabra()

letras_adivinadas  = []

intentos  =  10

  

print("¡Bienvenido al juego del ahorcado!")

while  True:

display_actual  =  mostrar_palabra(palabra_a_adivinar, letras_adivinadas)

print("\nPalabra a adivinar:", display_actual)

if  display_actual  ==  palabra_a_adivinar:

print("\n¡Felicidades! ¡Has adivinado la palabra!")

break

if  intentos  ==  0:

print("\n¡Te has quedado sin intentos! La palabra era:", palabra_a_adivinar)

break

adivinanza  =  input("\nIngresa una letra: ").lower()

if  len(adivinanza) !=  1  or  not  adivinanza.isalpha():

print("Por favor, ingresa una sola letra válida.")

continue

if  adivinanza  in  letras_adivinadas:

print("Ya has adivinado esa letra.")

continue

letras_adivinadas.append(adivinanza)

if  adivinanza  in  palabra_a_adivinar:

print("¡Correcto! La letra está en la palabra.")

else:

intentos  -=  1

print("Incorrecto. Te quedan", intentos, "intentos.")

if  __name__  ==  "__main__":

main()


}

# c++ ahorcado

#include <iostream>
using namespace std;

int main() {
    string palabra = "hola mundo";
    string palabraAdivinada(palabra.length(), '_');
    int intentos = 5;

    while (intentos > 0 && palabraAdivinada != palabra) {
        cout << "Palabra: " << palabraAdivinada << endl;
        char letra;
        cout << "Ingresa una letra: ";
        cin >> letra;

        bool acierto = false;
        int i;
        for ( i = 0; i < palabra.length(); ++i) {
            if (palabra[i] == letra || palabra[i] == ' ') {
                palabraAdivinada[i] = palabra[i];
                acierto = true;
            }
        }

        if (!acierto) {
            cout << "Incorrecto. Te quedan " << intentos - 1 << " intentos." << endl;
            intentos--;
        }
    }

    if (palabraAdivinada == palabra) {
        cout << "¡Felicidades, adivinaste la palabra: " << palabra << "!" << endl;
    } else {
        cout << "¡Agotaste tus intentos! La palabra era: " << palabra << endl;
    }

    return 0;
}


# Video de codigos y funcionamiento
[https://youtu.be/WsEL17vvQMg]()
---





|*Christian Alejandro Conde Lemus*|
 ----------------------------------------------------------------
  |7690-19-11539 |
  ------------------------------------------------------------
  |(Ahorcado y Pitagoras en Python, archivo Markdown, video)|
  -----------------------------------------------------
|*Juan Jose Arevalo Patzan*|
-----------------------------------------------------------------
| 7690-21-15416|
-----------------------------------------------------------------
| (Ahorcado y Pitagoras en c++ y Pseudocodigo, edición de video, Hithub)  |

>Algoritmos Seccion D

