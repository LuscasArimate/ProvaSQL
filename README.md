# PROVA PRATICA SQL


<h1 align="center"> Bem vindos  👋</h1>
<h3 align="center">Prova pratica de SQL  </h3>
<h3 align="center"> By Luscas_arimate   </h3>


<h3 align="left">Antes de tudo </h3>
<p align="left">  Abra o arquivo "bdescola.txt" acima e execute no PostgreSQL, utilizando a ferramenta PgAdmin4 no seu computador. Nao esqueça de criar um Banco chamado "bdescola" clicabdo com o botao direito em " DATABASES " no PostgreSQL



<h3 align="left">Resultado esperado </h3>

![Captura de tela 2022-12-07 145632](https://user-images.githubusercontent.com/93049848/206259633-7270bb92-8a52-43d5-be3c-a50d524fb08e.png)

![Captura de tela 2022-12-07 145653](https://user-images.githubusercontent.com/93049848/206259641-9d354b91-1640-4489-b524-cdeef89da38f.png)

![Captura de tela 2022-12-07 145607](https://user-images.githubusercontent.com/93049848/206259644-30eb0c77-30bd-4502-b66a-863e0890c9dd.png)

### QUESTAO 1 

```SQL


INSERT INTO TB_ALUNO(CODIGO_ALUNO, NOME_ALUNO,ANO_NASC, EMAIL, SEXO)

VALUES (4,'Pedro Cesar', NULL, NULL, 'M');

INSERT INTO TB_MATRICULA( CODIGO CURSO, CODIGO_ALUNO)
VALUES (4,4)


```
![quest1(1-2)](https://user-images.githubusercontent.com/93049848/206260508-981bca26-a847-493e-af39-e0bdeaba8c3e.png)

![quest1(2-2)](https://user-images.githubusercontent.com/93049848/206260580-ba31f1ae-271a-4fb1-9949-bfbc2ce789b0.png)



### QUESTAO 2

```SQL

SELECT TB_ALUNO.NOME_ALUNO, TB_CURSO.NOME_CURSO 
FROM TB_ALUNO 
INNER JOIN TB_MATRICULA 
ON TB_ALUNO.CODIGO_ALUNO = TB_MATRICULA.CODIGO_ALUNO
INNER JOIN TB_CURSO
ON TB_CURSO.CODIGO_CURSO = TB_MATRICULA.CODIGO_CURSO


```


### QUESTAO 3

```SQL

SELECT EMAIL
FROM TB_ALUNO WHERE 2022 - ANO_NASC >= 18



```
![quest3](https://user-images.githubusercontent.com/93049848/206262205-ad6965c1-5095-4bb4-b68a-9601a5660881.png)


