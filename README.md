package CLASSES;

public class funcionarios {
private String nome;
private int idade;
private double [] salarios;
private double media;

	public void dados(){
		System.out.println(this.nome);
		System.out.println(this.idade);
		System.out.println(this.salarios[0]);
		System.out.println(this.salarios[1]);
		System.out.println(this.salarios[2]);
}
	public void imprimeMedia() {
		this.media = 0;
		
		for(double salarios : this.salarios) {
			this.media+= salarios;
		}
		this.media/= this.salarios.length;
		System.out.println();
		System.out.println("media salarial " + this.media);
	}
	public void setnome(String nome) {
		this.nome = nome;
	}
	public void setidade(int idade) {
		this.idade = idade;
	}
	public void setsalarios(double salarios []) {
		this.salarios = salarios;
	}
	public String getnome() {
		return nome;
	}
	public int getidade() {
		return idade;
	}
	public double[] getsalarios() {
		return salarios;
	} 
	public double getmedia() {
		return media;
	}
}
