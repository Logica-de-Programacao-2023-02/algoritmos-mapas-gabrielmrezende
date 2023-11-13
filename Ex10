package main

import "fmt"

func contarPares(slice []int) map[[2]int]int {
	frequencias := make(map[[2]int]int)

	for i := 0; i < len(slice); i++ {
		for j := i + 1; j < len(slice); j++ {
			par := [2]int{slice[i], slice[j]}
			frequencias[par]++
		}
	}

	return frequencias
}

func main() {
	numeros := []int{1, 2, 3, 2, 1, 4, 5, 4}

	frequencias := contarPares(numeros)

	for par, frequencia := range frequencias {
		fmt.Printf("%v: %d\n", par, frequencia)
	}
}
