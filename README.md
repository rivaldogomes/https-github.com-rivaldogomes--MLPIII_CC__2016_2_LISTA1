# https-github.com-rivaldogomes--MLPIII_CC__2016_2_LISTA1
public class Fatura{
    private int quantidade;
    private String numero;
    private String descricao;
    private double preco;
   
    Fatura(){}
    Fatura(int quantidade, String numero, String descricao, double preco){
        this.numero=numero;
        this.quantidade=quantidade;
        this.descricao=descricao;
        this.preco=preco;
    }
   
    public void setNumero(int numero){
        this.numero=numero;
    }
    public void setQuantidade(int quantidade){
        this.quantidade=quantidade;
    }
    public void setDescricao(String descricao){
        this.descricao=descricao;
    }
    public void setPreco(double preco){
        this.preco=preco;
    }
   
    public int getNumero(){
        return numero;
    }
    public int getQuantidade(){
        return quantidade;
    }
    public String getDescricao(){
        return descricao;
    }   
    public double getPreco(){
        return preco;
    }

    public double getValorFaturaAmount(){
        double amount = preco*quantidade;
        if(quantidade<0){ this.quantidade=0; }
        if(preco<0){this.preco=0.0;}
        return amount;
    }
}
