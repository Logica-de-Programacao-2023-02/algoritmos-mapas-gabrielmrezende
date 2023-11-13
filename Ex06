package main

import "fmt"

func ContagensDeMapas(listaDeMapas []map[string]int) map[string]int {
	resultado := make(map[string]int)

	for _, mapa := range listaDeMapas {
		for palavra, contagem := range mapa {
			resultado[palavra] += contagem
		}
	}

	return resultado
}

func main() {
	mapa1 := map[string]int{"apple": 2, "banana": 3, "cherry": 1}
	mapa2 := map[string]int{"apple": 1, "cherry": 2, "date": 4}
	mapa3 := map[string]int{"banana": 2, "date": 3}

	listaDeMapas := []map[string]int{mapa1, mapa2, mapa3}

	resultado := ContagensDeMapas(listaDeMapas)

	for palavra, contagem := range resultado {
		fmt.Printf("%s: %d\n", palavra, contagem)
	}
}
