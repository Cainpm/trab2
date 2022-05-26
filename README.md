 static void provaAI(double[] notas) {
	        double notaAi = 0;
	        int piorNota = notas[0] <= notas[1] ? 0 : 1; //Verifica a menor entre as 2 primeira notas.


	        System.out.println("Digite A Nota Da Prova AI");
	        notaAi = lerNota("Prova AI", NOTA_MAX_AVALIACOES[piorNota]);

	        if (notaAi > notas[piorNota]) {
	            notas[piorNota] = notaAi;
	            System.out.printf("A Avaliação %s Foi Substituida Pela Avalição AI\n", NOME_AVALIACOES[piorNota]);
	        } else {
	            System.out.println("A Nota Da Prova AI Não Foi Suficiente Para Alterar Alguma Prova");
	        }

	    } // Fim do método provaAI()
