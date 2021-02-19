# Ordena-o_lg2

1
package  ordenação_lg2 ;


 classe  pública Ordena ção_1 {


	public  static  void  main ( String [] args ) {


		vetor int [] = { 3 , 6 , 2 , 1 , 8 , 4 };


		int aux;


		controle booleano ;


		para ( int i =  0 ; i < vetor . comprimento; ++ i) {


			controle =  verdadeiro ;


			for ( int j =  0 ; j < (vetor . comprimento -  1 ); ++ j) {


				se (vetor [j] > vetor [j +  1 ]) {


					aux = vetor [j];


					vetor [j] = vetor [j +  1 ];


					vetor [j +  1 ] = aux;


					controle =  falso ;


				}


			}


				if (controle) {


					pausa ;


				}


			}



		para ( int i =  0 ; i < vetor . comprimento; ++ i) {


			Sistema . para fora . println (vetor [i] +  " " );	


		}




	}



}



2

package  ordenação_lg2 ;



import  java.util.Arrays ;


import  java.util.Random ;


 classe  pública Ordena ção_2 {



	public  static  void  main ( String [] args ) {


		int [] v = gerarVetor ( 10 );


		selectionSort (v);


		Sistema . para fora . println ( Arrays . toString (v));


	}



	private  static  void  selectionSort ( int [] v ) {


		para ( int i =  0 ; i < v . comprimento; i ++ ) {


			int menor = i;


			para ( int j = i +  1 ; j < v . comprimento; j ++ ) {


				if (v [j] < v [menor])


					menor = j;


			}


			trocar (v, i, menor);


		}


	}


	 trocarte privado estático  vazio  ( int [] v , int i , int menor ) {  


		int aux = v [i];


		v [i] = v [menor];


		v [menor] = aux;


	}



	public  static  int [] gerarVetor ( int  n ) {


	int [] v =  novo  int [n];


	Gerador aleatório =  novo  Random ();


	para ( int i =  0 ; i < n; i ++ ) {


		v [i] = gerador . nextInt ( 100 );


	}


	return v;


	}


}


3 


package  ordenação_lg2 ;


public  class  Recurs ão {


		public  static  int  fatorialNaoRecursivo ( int  num ) {


			if (num ==  0 ) {


				return  1 ;


			}


			total int =  1 ;


			para ( int i = num; i >  1 ; i - ) {


				total * = i;


			}


			retorno total;


		}


		public  static  int  fatorial ( int  num ) {



			if (num ==  0 ) {


				return  1 ;


			}


			retornar num * fatorial (num - 1 );


		}

	}


