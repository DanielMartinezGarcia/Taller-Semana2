# Taller-Semana2

1. Una solucion contiene los elementos para crear una aplicacion, un ensamble es el ejecutable con 
varios archivos y un proyecto sirve para organizar de manera logica los elementos dentro de una solucion.

2. el using system sirve para ejecutar librerias y pedazos de codigo que estan dentro de la aplicacion.

3. Son estructuras que agrupan campos y metodos.

4. El unsigned almacena datos positivos y el SIGNED no solo almacena positivos sino tambien negativos.

5. Sbyte esta por fuera del rango-

6. Los tipo SHORT almacenan menor cantidad de valores a diferencia de los INT.

7. Si.

8. SIrve para diferenciar el tipo de variable que es ese numero.

9. El programa espera que le entren algun tipo de dato para leerlo.

10. Convierte un tipo de dato base a otro tipo de dato base.

11. Console.WriteLine("C:\Users\juanfh\Desktop\MiArchivo.txt"); //el backslash es un caracter de escape por eso para que el programa lo reconozca hay que poner doble backslash.

12. La variable tipo SHORT se desborda del rango.

13. En la primera linea define la variable y en la segunda le asigna un valor.

14. Es un arreglo con 10 caracteres.

15. El micropocesador toma nota y sabe a que direccion dirigirse.

16. En el Stack.

17. El heap se almacena las clases y se van borrando con el garbage collector si no se necesaita.
eso se hace automaticamente.

18. Como el stack sirve para almacenar variables locales, La variable Message queda almacenada alli.
Mientras la cadena "hello" queda almacenada en el Heap.
el heap sirve para almacenar variable type referencia, clases, objetos, etc. como los string son tipo referencia 
y crea un objeto debido a esto va al heap.

19. La variable local message queda almacenada en el stack. mientras que en el heap se crea un arreglo en el que contiene tres 
objetos, al ser tres objetos se crea un espacio aparte en el heap a cada uno, por lo tanto en el array queda almacenada las 
tres direcciones de los objetos en el heap.

20. La variable local numbers se almacena en el stack, en el heap queda el arreglo y dentro del arreglo contiene las variables y 
como son tipo value se incluyen dentro del array.

22. Por ser Int son tipo value y se almacena en el Stack.

23. En El heap queda almacenado en el array, y al ser tipo referencia, "a" y "b" apuntan a la misma direccion y imprimen el valor
de 17.

24. Se crea una clase MyInt , contiene un atributo con dos metodos, en el primero se crea un metodo con dos variables
en donde la segunda toma el valor de la primera.En el segudo metodo se crea una variable del tipo de la clase creada al inicio y cuando se le ve a asignar un valor a esa variable se usa la variable de que esta adentro de la clase lo cual modifica la variable adentro de la clase, luego se crea una segunda variable del mismo tipo de la clase creada al inicio esta vez cuando se le va a dar el valor a esta variable se le da el mismo valor de "x" y
como "x" tiene la direccion de MyValue al modificar "y" estamos modificando "x" que modifica a MyValue.

25. por que se inicializa el constructor.

this.tittle = tittle.

para diferenciar variable que estan afuera.

26. no, por que x esta incluido dentro del for.

27. Con el THIS podemos diferenciar dos variable con el mismo nombre, y adema sirve para acceder a la clase incluso si es 
Private.

28. separa una palabra por espacios y luego cuenta cada una.

30.
struct. tipo valor. Stack. se guarda la estructura completa en el stack.
class. tipo referencia. heap.

31.
el tipo class se guarda en el heap y los tipo struct en el stack

C1. using System;

namespace RetoUno
{
	public class Reto2
	{
		public Reto2 ()
		{
			string radio = "";
			string altura = "";
			double volumen = 0;
			double area = 0;

			Console.WriteLine ("Escriba  el radio:");
			radio = Console.ReadLine ();
			double r = double.Parse (radio);

			Console.WriteLine ("Escriba la altura:");
			altura = Console.ReadLine ();
			double a = double.Parse (altura);

			area = r * r * Math.PI;
			volumen = area * a;

			Console.WriteLine ("el area es: {0} y el volumen es {1}", area, volumen);
			Console.ReadKey ();



		}
	}
}

C2. int a = 7;
        int b = 2;
        float c = 4;
        float d = 3;

        float result = ((float)(a)/(float)(b)) + c / d;
        Console.WriteLine("resultado: {0}",result);
Para convertirlo en float.

C3.
int[] numeros = {4, 51, -7, 13, -99, 15, -8, 45, 90};
        int menor = 0;
        int mayor = 0;

        foreach (int numero in numeros)
        {
            if (menor > numero)
            {
                menor = numero;
            }

            if (mayor < numero)
            {
                mayor = numero;
            }
        }

        Console.WriteLine("El mayor es {0} y el menor es {1}", mayor , menor);
        
      
c4. 
using System;

namespace Application
{
	public class C4_Reto_
	{
		public C4_Reto_ ()
		{
			string Numero = "";
			Console.WriteLine ("Escriba un numero entre el 1 al 7");
			Numero = Console.ReadLine();
			int num = int.Parse (Numero);

			switch (Numero) 
			{
			case 1:
				Console.WriteLine ("el dia es {0}", sabado);
				break;

			case 2:
				Console.WriteLine ("el dia es {0}", domingo);
				break;
			case 3:
				Console.WriteLine ("el dia es {0}", lunes);
				break;
			case 4:
				Console.WriteLine ("el dia es {0}", martes);
				break;
			case 5:
				Console.WriteLine ("el dia es {0}", miercoles);
				break;
			case 6:
				Console.WriteLine ("el dia es {0}", jueves);
				break;

			case 7:
				Console.WriteLine ("el dia es {0}", viernes);
				break;

			default:
				break;

			

		}
	}
}

c5. 
se crea una estructura tipo time en el stack. y un timestruct tipo 
class en el heap y se vuelve a crear otro mismo. pero cuando le damos return se vuelve al valor inicial 10.



