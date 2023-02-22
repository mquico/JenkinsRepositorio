def variable1= 10
def variable2= 20
pipeline
{
    agent any
    stages
    {
        stage ("Creacion de Archivo")
        {
            steps
            {
                script
                {
                    def multiplicacion = variable1*variable2
                    def suma = variable1+variable2
                    def potencia = suma*suma
                    
                    
                    
                    println "Variable 1: " + variable1
                    println "Variable 2: " + variable2
                    println "Multiplicación: " + multiplicacion
                    println "Suma de potencias: " + potencia
                    
                    def informacion = "Multiplicación: " + multiplicacion
                    informacion+="\nSuma de pontencia: " + potencia
                    
                    writeFile(file: "C:\\quico\\salida.txt", text: informacion)
                }
            }
        }
    }
}
