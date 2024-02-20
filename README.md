- 👋 Hi, I’m @Diego20006
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Diego20006/Diego20006 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
1. librería que me permita realizar tres funciones específicas en java

1.	Función para calcular el área de un círculo:
2.	Función para calcular el área de un rectángulo:
3.	Función para verificar si un número es primo:
 
public class MisFunciones {
    
    // Función para calcular el área de un círculo
    public static double calcularAreaCirculo(double radio) {
        return Math.PI * radio * radio;
    }
    
    // Función para calcular el área de un rectángulo
    public static double calcularAreaRectangulo(double base, double altura) {
        return base * altura;
    }
    
    // Función para verificar si un número es primo
    public static boolean esPrimo(int numero) {
        if (numero <= 1) {
            return false;
        }
        for (int i = 2; i <= Math.sqrt(numero); i++) {
            if (numero % i == 0) {
                return false;
            }
        }
        return true;
    }
}

2.librería en java que me permita operar un trinomio cuadrado perfecto
public class TrinomioCuadradoPerfecto {
    
    // Método para calcular el primer término del trinomio (a^2)
    public static int calcularPrimerTermino(int a) {
        return a * a;
    }
    
// Método para calcular el segundo término del trinomio (2ab)
public static int calcularSegundoTermino(int a, int b) {
return 2 * a * b;
}
    
    // Método para calcular el tercer término del trinomio (b^2)
    public static int calcularTercerTermino(int b) {
        return b * b;
    }
    
    // Método para verificar si un trinomio es cuadrado perfecto
    public static boolean esCuadradoPerfecto(int a, int b) {
        int discriminante = b * b - 4 * a;
        return discriminante == 0;
    }
    
    // Método para encontrar las raíces del trinomio
    public static double[] encontrarRaices(int a, int b) {
        double discriminante = b * b - 4 * a;
        if (discriminante < 0) {
            return new double[0]; // No hay raíces reales
        } else if (discriminante == 0) {
            double raiz = -b / (2.0 * a);
            return new double[] { raiz };
        } else {
            double raiz1 = (-b + Math.sqrt(discriminante)) / (2.0 * a);
            double raiz2 = (-b - Math.sqrt(discriminante)) / (2.0 * a);
            return new double[] { raiz1, raiz2 };
        }
    }
}


