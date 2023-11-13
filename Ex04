package main

import (
	"fmt"
	"sort"
	"strings"
)

func ordenar(palavra string) string {
	letras := strings.Split(palavra, "")
	sort.Strings(letras)
	return strings.Join(letras, "")
}

func Anagramas(palavras []string) map[string][]string {
	anagramas := make(map[string][]string)

	for _, palavra := range palavras {
		chave := ordenar(palavra)
		anagramas[chave] = append(anagramas[chave], palavra)
	}

	return anagramas
}

func main() {
	palavras := []string{"amor", "roma", "carro", "corra", "cão", "não", "lar", "ral"}

	gruposAnagramas := Anagramas(palavras)

	for chave, grupo := range gruposAnagramas {
		fmt.Printf("%s: %v\n", chave, grupo)
	}
}
