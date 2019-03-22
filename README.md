# Título del trabajo

Descripción breve del proyecto a realizar (2-3 frases).

## Integrantes del equipo

* Noelia Arencibia Jaramillo,  @ajnoelia 
* Wasima Simouh  Majid,  @WasimaSimouh 
* Paula Alejandra  Mantilla,  @alepau

## Objetivos del trabajo

Lista de los objetivos que se persiguen con el trabajo propuesto.
## Menu de opciones
//AGENCIA DE VIAJES 
//MENU
#include<stdio.h>
#include <stdlib.h>

int main()
{
	system("color 4F");
  char Origen[40], Destino[40], respRegist;
	char Nombre[30], Apellido1[30], Apellido2[30];
	char CorreoElec[200], Contrasena[50];
	int NumPasajeros;
	int DD1, MM1, AA1, DD2, MM2, AA2;
	char opcionderegistrado;
	printf("Introduzca su origen:\n");
	scanf("%s", Origen);
	
  fflush(stdin);
	printf("Introduzca el destino:\n");
	scanf("%s", Destino);
	fflush(stdin);
	printf("Introduzca la fecha de ida (DD/MM/AA):\n");
	scanf("%d %d %d", &DD1, &MM1, &AA1);
	fflush(stdin);
	
  printf("Introduzca la fecha de vuelta(DD/MMM/AA):\n");
	scanf("%d %d %d", &DD2, &MM2, &AA2);
	fflush(stdin);
	
  printf("Introduzca el n%cmero de pasajeros:\n", 163);
	scanf("%d", &NumPasajeros);
		do{
		printf("¿Está usted registrado en nuestra agencia? (S,N,E)\n");
	scanf("%c",&opcionderegistrado);
	fflush(stdin);
	
   switch(opcionderegistrado)
	{
		case 'S':
		{
			printf("Para responder si 'S'y para responder no 'N' y salir 'E'");
			printf("Escriba su contraseña:\n");
			gets(Contrasena);
			printf("Mientras comprobamos su contrase%ca, nos encontramos buscando los mejores vuelos para usted ,familia y amigos!\n",                       
      164);
			printf("Espere un momento\n");
		break;
		}
	 	case 'N':
		{
			printf("Escriba su nombre, por favor:\n");
			scanf("%s", Nombre);
			printf("Ahora, escriba sus apellidos:\n");
			scanf("%s %s", Apellido1, Apellido2 );
			printf("Escriba su correo electr%cnico para poder enviarle ofertas, informaci%cn sobre su vuelo...\n", 162, 162);
			gets(CorreoElec);
			printf("Por %cltimo, escriba una contrase%ca segura para acabar de configurar su cuenta:\n", 163, 164);
			gets(Contrasena);
			break;
		}
		case 'E':
		{
			printf("Vuelva pronto!\n");
			printf("RECUERDE, VIAJAR ALIMENTA EL ALMA!\n");
			break;
		}
	}
}while(opcionderegistrado!='E');
	
   return 0;
}
