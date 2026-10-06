INICIO

    datos ← [
        ["Ana garcia", "6861234501"],
        ["Andrea lopez", "6861234502"],
        ["Antonio hernandez", "6861234503"],
        ["Beatriz martinez", "6861234504"],
        ["Brenda ramirez", "6861234505"],
        ["Carlos gonzalez", "6861234506"],
        ["Carolina torres", "6861234507"],
        ["Carmen flores", "6861234508"],
        ["Daniel rivera", "6861234509"],
        ["David sanchez", "6861234510"],
        ["Diego castro", "6861234511"],
        ["Eduardo mendoza", "6861234512"],
        ["Elena ortiz", "6861234513"],
        ["Emilio morales", "6861234514"],
        ["Fernando jimenez", "6861234515"],
        ["Francisco ruiz", "6861234516"],
        ["Gabriela diaz", "6861234517"],
        ["Gerardo vargas", "6861234518"],
        ["Guadalupe navarro", "6861234519"],
        ["Hector ramirez", "6861234520"],
        ["Isabel moreno", "6861234521"],
        ["Javier munoz", "6861234522"],
        ["Jesus alvarez", "6861234523"],
        ["Jimena romero", "6861234524"],
        ["Jorge gutierrez", "6861234525"],
        ["Jose dominguez", "6861234526"],
        ["Juan vasquez", "6861234527"],
        ["Laura ramos", "6861234528"],
        ["Leonardo vazquez", "6861234529"],
        ["Leticia herrera", "6861234530"],
        ["Luis mendoza", "6861234531"],
        ["Manuel medina", "6861234532"],
        ["Marco aguilar", "6861234533"],
        ["Maria vega", "6861234534"],
        ["Mariana castillo", "6861234535"],
        ["Mario cortes", "6861234536"],
        ["Miguel santos", "6861234537"],
        ["Monica ortega", "6861234538"],
        ["Natalia delgado", "6861234539"],
        ["Nicolas perez", "6861234540"],
        ["Patricia silva", "6861234541"],
        ["Paola espinoza", "6861234542"],
        ["Raul salazar", "6861234543"],
        ["Ricardo ponce", "6861234544"],
        ["Roberto cabrera", "6861234545"],
        ["Rosa maldonado", "6861234546"],
        ["Santiago valdez", "6861234547"],
        ["Sofia corona", "6861234548"],
        ["Victor acosta", "6861234549"],
        ["Ximena mendoza", "6861234550"]
    ]

    objetivo ← "Luis mendoza"

    izquierda ← 0
    derecha ← 49

    encontrado ← FALSO

    MIENTRAS izquierda ≤ derecha Y encontrado = FALSO HACER

        medio ← (izquierda + derecha) DIV 2

        SI datos[medio][0] = objetivo ENTONCES

            telefono ← datos[medio][1]
            encontrado ← VERDADERO

        SINO SI datos[medio][0] < objetivo ENTONCES

            izquierda ← medio + 1

        SINO

            derecha ← medio - 1

        FIN SI

    FIN MIENTRAS

    SI encontrado = VERDADERO ENTONCES
        IMPRIMIR telefono
    SINO
        IMPRIMIR "Nombre no encontrado"
    FIN SI

FIN