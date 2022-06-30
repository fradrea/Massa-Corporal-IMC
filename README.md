programa
{
   
   funcao inicio()
   {
        cadeia resultado = calcularImc(47, 1.60, 80.2)
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
        
        se (imc >= 25 e imc < 30) 
        {
            resultado = "você está acima do peso."
        }
        
        se (imc >= 30 e imc < 35) 
        {
            resultado = "você está com sobrepeso."
        }
        
        se (imc >= 35 e imc < 40) 
        {
            resultado = "você está com obesidade."
        }
        
        se (imc >= 40) 
        {
            resultado = "você está com obesidade grave."
        }
        
        retorne "Seu IMC é " + imc + " e " + resultado
    }

}
