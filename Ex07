package main

import (
	"fmt"
	"strings"
)

func contarLetras(palavra string) map[rune]int {
	contagem := make(map[rune]int)

	for _, char := range palavra {
		if char != ' ' {
			contagem[char]++
		}
	}

	return contagem
}

func contarLetrasNasPalavras(frase string) map[string]map[rune]int {
	palavras := strings.Fields(frase)
	resultado := make(map[string]map[rune]int)

	for _, palavra := range palavras {
		resultado[palavra] = contarLetras(palavra)
	}

	return resultado
}

func main() {
	frase := "Olá mundo, como está você?"

	resultado := contarLetrasNasPalavras(frase)

	for palavra, contagem := range resultado {
		fmt.Printf("%s:\n", palavra)
		for letra, quantidade := range contagem {
			fmt.Printf("    %c: %d\n", letra, quantidade)
		}
	}
}
