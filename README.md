1) Simulando um sistema escolar, crie um algoritmo em Java que receba do aluno as 8 notas
anuais. O algoritmo deve calcular as médias bimestrais, as médias semestrais, e a média final.
Ao final dos cálculos, o algoritmo deve apresentar os resultados de forma clara. (VERSÃO SEM
USO DE FOR E ARRAY).
import java.util.Scanner;
public class Questao_1 {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Entrada das 8 notas
 System.out.print("Digite a nota do 1º mensal: ");
 double nota1 = scanner.nextDouble();
 System.out.print("Digite a nota do 2º mensal: ");
 double nota2 = scanner.nextDouble();
 System.out.print("Digite a nota do 3º mensal: ");
 double nota3 = scanner.nextDouble();
 System.out.print("Digite a nota do 4º mensal: ");
 double nota4 = scanner.nextDouble();
 System.out.print("Digite a nota do 5º mensal: ");
 double nota5 = scanner.nextDouble();
 System.out.print("Digite a nota do 6º mensal: ");
 double nota6 = scanner.nextDouble();
 System.out.print("Digite a nota do 7º mensal: ");
 double nota7 = scanner.nextDouble();
 System.out.print("Digite a nota do 8º mensal: ");
 double nota8 = scanner.nextDouble();
 // Cálculo das médias bimestrais do 1º semestre
 double bimestre1 = (nota1 + nota2) / 2;
 double bimestre2 = (nota3 + nota4) / 2;
 double semestre1 = (bimestre1 + bimestre2) / 2;
 // Cálculo das médias bimestrais do 2º semestre
 double bimestre3 = (nota5 + nota6) / 2;
 double bimestre4 = (nota7 + nota8) / 2;
 double semestre2 = (bimestre3 + bimestre4) / 2;
 double mediaFinal = (semestre1 + semestre2) / 2;
 // Saída dos resultados
 System.out.println("\nRESULTADO FINAL");
 System.out.println("----------------------");
 System.out.printf("1º Bimestre: %.1f\n", bimestre1);
 System.out.printf("2º Bimestre: %.1f\n", bimestre2);
 System.out.printf("1º Semestre: %.1f\n", semestre1);
 System.out.println("----------------------");
 System.out.printf("3º Bimestre: %.1f\n", bimestre3);
 System.out.printf("4º Bimestre: %.1f\n", bimestre4);
 System.out.printf("2º Semestre: %.1f\n", semestre2);
 System.out.println("----------------------");
 System.out.printf("Média Final: %.1f\n", mediaFinal);
 }
}
1) Simulando um sistema escolar, crie um algoritmo em Java que receba do aluno as 8 notas
anuais. O algoritmo deve calcular as médias bimestrais, as médias semestrais, e a média final.
Ao final dos cálculos, o algoritmo deve apresentar os resultados de forma clara. (VERSÃO COM
UTILIZAÇÃO DO FOR E ARRAY).
import java.util.Scanner;
public class Questao_1 {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Array para armazenar as 8 notas
 double[] notas = new double[8];
 // Entrada das notas
 for (int i = 0; i < 8; i++) {
 System.out.print("Digite a nota do " + (i + 1) + "º mensal: ");
 notas[i] = scanner.nextDouble();
 }
 // Cálculo das médias bimestrais do 1º semestre
 double bimestre1 = (notas[0] + notas[1]) / 2;
 double bimestre2 = (notas[2] + notas[3]) / 2;
 double semestre1 = (bimestre1 + bimestre2) / 2;
 // Cálculo das médias bimestrais do 2º semestre
 double bimestre3 = (notas[4] + notas[5]) / 2;
 double bimestre4 = (notas[6] + notas[7]) / 2;
 double semestre2 = (bimestre3 + bimestre4) / 2;
 // Média final
 double mediaFinal = (semestre1 + semestre2) / 2;
 // Saída dos resultados
 System.out.println("\nRESULTADO FINAL");
 System.out.println("----------------------");
 System.out.printf("1º Bimestre: %.1f\n", bimestre1);
 System.out.printf("2º Bimestre: %.1f\n", bimestre2);
 System.out.printf("1º Semestre: %.1f\n", semestre1);
 System.out.println("----------------------");
 System.out.printf("3º Bimestre: %.1f\n", bimestre3);
 System.out.printf("4º Bimestre: %.1f\n", bimestre4);
 System.out.printf("2º Semestre: %.1f\n", semestre2);
 System.out.println("----------------------");
 System.out.printf("Média Final: %.1f\n", mediaFinal);
 scanner.close();
 }
}
2) Desenvolva um algoritmo em Java que receba como entrada uma temperatura em graus
Celsius (°C) digitada pelo usuário. O programa deverá realizar a conversão dessa temperatura
para as escalas Fahrenheit (°F) e Kelvin (K), utilizando as seguintes fórmulas de conversão:
Fahrenheit (°F) = (Celsius (°C) × 9/5) + 32
Kelvin (K) = Celsius (°C) + 273.15
Ao final dos cálculos, o algoritmo deve exibir na tela o valor da temperatura original em
Celsius, juntamente com os valores convertidos em Fahrenheit e Kelvin, de forma clara e
informativa.
import java.util.Scanner;
public class Questao_2 {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Entrada da temperatura em Celsius
 System.out.print("Digite a temperatura em Celsius (°C): ");
 double celsius = scanner.nextDouble();
 // Conversões
 double fahrenheit = (celsius * 9 / 5) + 32;
 double kelvin = celsius + 273.15;
 // Saída formatada dos resultados

 System.out.printf("Temperatura em Celsius: %.2f °C\n", celsius);
 System.out.printf("Temperatura em Fahrenheit: %.2f °F\n", fahrenheit);
 System.out.printf("Temperatura em Kelvin: %.2f K\n", kelvin);
 }
}
