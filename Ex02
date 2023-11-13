package main

import "fmt"

func mergeMaps(map1, map2 map[string]int) map[string]int {
	Map := make(map[string]int)

	for chave, valor := range map1 {
		Map[chave] = valor
	}

	for chave, valor := range map2 {
		Map[chave] = valor
	}

	return Map
}

func main() {
	mapa1 := map[string]int{"a": 1, "b": 2, "c": 3}
	mapa2 := map[string]int{"b": 4, "d": 5, "e": 6}

	resultado := mergeMaps(mapa1, mapa2)

	for chave, valor := range resultado {
		fmt.Printf("%s: %d\n", chave, valor)
	}
}
