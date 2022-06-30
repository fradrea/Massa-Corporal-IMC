programa
{
    
    funcao inicio()
    
    {
        cadeia resultado = calcularImc( 39, 1.75, 89.2)
        escreva(resultado)
    }

    funcao cadeia calcularImc(inteiro idade, real altura, real peso)
    {
        cadeia resultado = ""
        real imc = peso/(altura * altura)
        
        se (imc <= 0) 
        {
            resultado = "IMC inválido!"
        }
        
        se (imc > 0 e imc < 18.5) 
        {
            resultado = "você está abaixo do peso."
        }
        
        se (imc >= 18.5 e imc < 25) 
        {
            resultado = "você está no peso normal."
        }
