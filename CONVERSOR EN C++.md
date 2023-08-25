#include<iostream>
using namespace std;

int main() {
	float longitudconvertida;
	float longitudencentimetros;
	float mtxcm;
	int opcion;
	float plxcm;
	float pxcm;
	float vrxcm;
	float yxcm;

	// definir las variables 
	// MTxCM= METROS X CENTIMETROS
	// PLxCM= PULGADAS X CENTIMETROS
	// PxCM= PIES X CENTIMETROS
	// YxCM= YARDAS X CENTIMETROS
	// VRxCM= VARAS X CENTIMETROS 

	mtxcm = 0.01;
	plxcm = 0.393701;
	pxcm = 0.0328094;
	yxcm = 0.0109361;
	vrxcm = 0.011904761;

	cout << "Ingresar longitud en centimetros:" << endl;
	cin >> longitudencentimetros;

	// Solicitar al usuario seleccionar la unidad de conversion
	cout << "Que conversion deseas hacer pon el numero segun a que medida quieras hacerlo:" << endl;
	cout << "1. Metros" << endl;
	cout << "2. Pulgadas" << endl;
	cout << "3. Pies" << endl;
	cout << "4. Yardas" << endl;
	cout << "5. Varas" << endl;
	cin >> opcion;
	
	// Realizar la conversion basada en la opcion seleccionada
	switch (opcion) {
	case 1:
		longitudconvertida = longitudencentimetros*mtxcm;
		break;
	case 2:
		longitudconvertida = longitudencentimetros*plxcm;
		break;
	case 3:
		longitudconvertida = longitudencentimetros*pxcm;
		break;
	case 4:
		longitudconvertida = longitudencentimetros*yxcm;
		break;
	case 5:
		longitudconvertida = longitudencentimetros*vrxcm;
		break;
	default:
		cout << "Por favor escriba un numero de opcion del 1 al 5" << endl;
	}
	// Mostrar el resultado de la conversion
	cout << "Conversion:" << longitudconvertida << "" << endl;
	return 0;
} 