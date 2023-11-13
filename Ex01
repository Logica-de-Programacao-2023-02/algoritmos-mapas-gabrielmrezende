package main

import (
	"fmt"
	"strings"
)

func contarPalavras(texto string) map[string]int {
	palavras := strings.Fields(texto)

	contagemPalavras := make(map[string]int)

	for _, palavra := range palavras {
		if _, existe := contagemPalavras[palavra]; existe {
			contagemPalavras[palavra]++
		} else {
			contagemPalavras[palavra] = 1
		}
	}

	return contagemPalavras
}

func main() {
	texto := "Esta é uma string de exemplo. Esta string contém palavras repetidas."
	contagem := contarPalavras(texto)

	for palavra, quantidade := range contagem {
		fmt.Printf("%s: %d\n", palavra, quantidade)
	}
}
