# Saludos en Go

Este paquete proporciona una forma simple de obtener saludos personalizados en Go.

## Istalación
Ejecuta el siguiente comando para intalar el paquete:
```bash
go get -u github.com/rokemagik/greetings
```
## Uso
Aquí tienes un ejemplo de como utilizar el paquete en tu código:

```go
package main

import (
    "fmt"
    "github.com/rokemagik/greetings"
)

func main() {
    message, err := greetings.Hello("Emi")
    
    if err != nil {
        fmt.Println("Ocurrio un error: ", err)
        return
    }

    fmt.Println(message)
}

```
Este ejemplo importa el paquete github.com/rokemagik/greetings y llama a la funcion Hello para imprimir un saludo personalizado. Si ocurre un error, se imprime un mensaje de error.