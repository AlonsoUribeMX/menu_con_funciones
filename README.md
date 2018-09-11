# menu_con_funciones
ciclo_do_while_en_java_Y_funciones_switch
import java.util.Scanner;
public class Main {
	public static void main (String [] argumentos) {
		int opcion;
		do {
		System.out.println("\tELIGUE UNA OPCION: \n 1.- AREA DE UN CUADRADO \n 2.- AREA DE UN RECTANGULO\n 3.- AREA DE UN TRIANGULO\n 4.- AREA DE UN CIRCULO \n 5.- SALIR DEL PROGRAMA");
		Scanner opc = new Scanner(System.in);
		opcion=opc.nextInt();		
		switch(opcion) {
    
		case 1:
			cuadrado();
			break;
			
		case 2: 
			rectangulo();
			break;
		case 3:
		    tria();
		break;
		case 4:
			circulo();
			break;
		case 5:
			System.out.println("*** GRACIAS POR USAR ESTE PROGRAMA ***");
			break;
		default:
			System.out.println(" ERROR OPCION INVALIDA , ELIGUE OTRA  ");
			break;	
		}
		}	
		while(opcion!=5);
	}
public static void cuadrado() {
	System.out.println("___________CUADRADO_____________");
	System.out.println("INGRESA LA MEDIDA DE UN LADO: ");
	Scanner leerlado= new Scanner(System.in);
	int lado=leerlado.nextInt();
	int area1=lado*lado;
	System.out.println("EL AREA ES: "+area1);
	}

public static void rectangulo () {
	System.out.println("___________RECTANGULO_____________");
	System.out.println("INGRESA LA MEDIDA DE UN LADO: ");
	Scanner leerlado= new Scanner(System.in);
	int lado=leerlado.nextInt();
	System.out.println("INGRESA LA BASE: ");
	Scanner leerbase= new Scanner(System.in);
	int base1=leerbase.nextInt();

	int area1=lado*base1;
	System.out.println("EL AREA ES: "+area1);
	
}


public static void tria () {
	

System.out.println("___________TRIANGULO_____________");	
System.out.println("INGRESA LA BASE: ");
Scanner leerbase= new Scanner(System.in);
int base1=leerbase.nextInt();

System.out.println("INGRESA LA ALTURA : ");
Scanner leeraltura= new Scanner(System.in);
int altura1=leeraltura.nextInt();
int area=(base1*altura1)/2;
System.out.println("EL AREA ES: "+area);}


public static void circulo () {
	
	System.out.println("___________CIRCULO_____________");
	System.out.println("INGRESA LA MEDIDA DEL RADIO: ");
	Scanner leerradio= new Scanner(System.in);
	int radio=leerradio.nextInt();
	double area3=(3.1416*radio)*radio;
	System.out.println("EL AREA ES: "+area3);}		
		
		
	}


