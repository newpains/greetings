# Saludos en GO
Este paquete proporciona una forma simple de obtener saludos personalizados en Go.

## Instalación
Ejecuta el siguiente comando para instalar el paquete:
```bash
go get -u github.com/newpains/greetings
```
## Uso
Aquí tienes un ejemplo de cómo utilizar el paquete en tu código:

```go
package main

import (
	"fmt"
	"github.com/newpains/greetings"
)

func main() {
	message, err := greetings.Hello("Martin")
	if err != nil {
		fmt.Println("Ocurrió un error:", err)
        return
	}
	fmt.Println(message)
}
```
Este ejemplo importa el paquete github.com/newpains/greetings y llama a la función Hello. Si ocurre un error se imprime un mensaje de error.
