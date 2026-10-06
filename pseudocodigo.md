INICIO

    datos ← [
        ["Ana garcia", "6861234501"],
        ["Andrea lopez", "6861234502"],
        ["Antonio hernandez", "6861234503"],
        ...
        ["Luis mendoza", "6861234531"],
        ...
        ["Ximena mendoza", "6861234550"]
    ]

    FUNCION busqueda_binaria(matriz, objetivo)

        izquierda ← 0
        derecha ← longitud(matriz) - 1

        MIENTRAS izquierda ≤ derecha HACER

            medio ← (izquierda + derecha) DIV 2

            clave ← matriz[medio][0]

            SI clave = objetivo ENTONCES
                RETORNAR matriz[medio][1]

            SINO SI clave < objetivo ENTONCES
                izquierda ← medio + 1

            SINO
                derecha ← medio - 1
            FIN SI

        FIN MIENTRAS

        RETORNAR NULO

    FIN FUNCION


    resultado ← busqueda_binaria(datos, "Luis mendoza")

    IMPRIMIR resultado

FIN