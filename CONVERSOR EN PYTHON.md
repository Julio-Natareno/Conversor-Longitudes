if __name__ == '__main__':

	# definir las variables 
	# MTxCM= METROS X CENTIMETROS
	# PLxCM= PULGADAS X CENTIMETROS
	# PxCM= PIES X CENTIMETROS
	# YxCM= YARDAS X CENTIMETROS
	# VRxCM= VARAS X CENTIMETROS 

	mtxcm = float()
	plxcm = float()
	pxcm = float()
	yxcm = float()
	vrxcm = float()

	# CUANTO EQUIVALE CADA UNIDAD A UN CENTIMETRO
	mtxcm = 0.01
	plxcm = 0.393701
	pxcm = 0.0328094
	yxcm = 0.0109361
	vrxcm = 0.011904761

	print "Ingresar longitud en centimetros:"
	longitudencentimetros = float(raw_input())

	# Solicitar al usuario seleccionar la unidad de conversion
	print "Que conversion deseas hacer pon el numero segun a que medida quieras hacerlo:"
	print "1. Metros"
	print "2. Pulgadas"
	print "3. Pies"
	print "4. Yardas"
	print "5. Varas"
	opcion = float(raw_input())
	
	# Realizar la conversion basada en la opcion seleccionada
	if opcion==1:
		longitudconvertida = longitudencentimetros*mtxcm
	elif opcion==2:
		longitudconvertida = longitudencentimetros*plxcm
	elif opcion==3:
		longitudconvertida = longitudencentimetros*pxcm
	elif opcion==4:
		longitudconvertida = longitudencentimetros*yxcm
	elif opcion==5:
		longitudconvertida = longitudencentimetros*vrxcm
	else:
		print "Por favor escriba un numero de opcion del 1 al 5"
	# Mostrar el resultado de la conversion
	print "Conversion:",longitudconvertida,""

