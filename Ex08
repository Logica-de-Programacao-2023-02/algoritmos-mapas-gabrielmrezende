package main

import (
	"fmt"
)

func Despesas(despesas map[string]float64) map[string]float64 {
	totalDespesas := 0.0
	for _, valor := range despesas {
		totalDespesas += valor
	}
	media := totalDespesas / float64(len(despesas))

	equalizacao := make(map[string]float64)
	for pessoa, valor := range despesas {
		diferenca := valor - media
		equalizacao[pessoa] = diferenca
	}

	return equalizacao
}

func main() {
	despesas := map[string]float64{
		"Alice": 40.0,
		"Bob":   30.0,
		"Carol": 50.0,
		"David": 20.0,
	}

	equal := Despesas(despesas)

	for pessoa, valor := range equal {
		fmt.Printf("%s deve receber/pagar: R$%.2f\n", pessoa, valor)
	}
}
