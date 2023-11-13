package main

import "fmt"

func contarCaracteres(texto string) map[rune]int {
	frequencia := make(map[rune]int)

	for _, char := range texto {
		frequencia[char]++
	}

	return frequencia
}

func main() {
	texto := "banana"
	frequencia := contarCaracteres(texto)

	for char, contagem := range frequencia {
		fmt.Printf("%c: %d\n", char, contagem)
	}
}
