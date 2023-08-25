Algoritmo ConversorDeLongitud
    
	//definir las variables 
	// MTxCM= METROS X CENTIMETROS
	//PLxCM= PULGADAS X CENTIMETROS
	//PxCM= PIES X CENTIMETROS
	//YxCM= YARDAS X CENTIMETROS
	//VRxCM= VARAS X CENTIMETROS 
	definir MTxCM Como Real
	definir PLxCM Como Real
	Definir PxCM Como Real
	DEFINIR YxCM Como Real
	DEFINIR VRxCM COMO REAL
	
	//CUANTO EQUIVALE CADA UNIDAD A UN CENTIMETRO
	MTxCM= 0.01
	PLxCM= 0.393701
	PxCM= 0.0328094
	YxCM= 0.0109361
	VRxCM= 0.011904761
	
	
    Escribir "Ingresar longitud en centimetros:"
	Leer longitudEnCentimetros
	
    // Solicitar al usuario seleccionar la unidad de conversion
    Escribir "Que conversion deseas hacer pon el numero segun a que medida quieras hacerlo:"
    Escribir "1. Metros"
    Escribir "2. Pulgadas"
    Escribir "3. Pies"
    Escribir "4. Yardas"
    Escribir "5. Varas"
    Leer opcion
	
    // Realizar la conversion basada en la opcion seleccionada
    Segun opcion Hacer
	1: longitudConvertida = longitudEnCentimetros * MTxCM
	2: longitudConvertida = longitudEnCentimetros * PLxCM
	3: longitudConvertida = longitudEnCentimetros * PxCM
	4: longitudConvertida = longitudEnCentimetros * YxCM
	5: longitudConvertida = longitudEnCentimetros * VRxCM
	De Otro Modo:
	Escribir "Por favor escriba un numero de opcion del 1 al 5"
	Fin Segun
	
    // Mostrar el resultado de la conversion
    Escribir "Conversion:", longitudConvertida,""
	
Fin Algoritmo

