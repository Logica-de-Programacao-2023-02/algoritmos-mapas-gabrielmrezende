package main

import "fmt"

func Sequencia(n int) map[int]int {
	sequencia := make(map[int]int)

	a, b := 0, 1
	for i := 0; a <= n; i++ {
		sequencia[i] = a
		a, b = b, a+b
	}

	return sequencia
}

func main() {
	n := 50
	sequencia := Sequencia(n)

	for indice, valor := range sequencia {
		fmt.Printf("%d: %d\n", indice, valor)
	}
}
