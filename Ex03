package main

import "fmt"

func somarValores(mapa map[string]int) int {
	soma := 0

	for _, valor := range mapa {
		soma += valor
	}

	return soma
}

func main() {
	mapa := map[string]int{
		"a": 1,
		"b": 2,
		"c": 3,
	}

	resultado := somarValores(mapa)

	fmt.Printf("A soma dos valores no mapa é: %d\n", resultado)
}
