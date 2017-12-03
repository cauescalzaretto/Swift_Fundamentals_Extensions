# Swift Fundamentals Extensions

    //: Playground - noun: a place where people can play
    
    import UIKit
    
    //---------------------------------------------------------------
    //: Author - Cauê Scalzaretto
    //: Site - http://www.cauescalzaretto.com
    //: GitHub - https://github.com/cauescalzaretto
    //---------------------------------------------------------------
    
    //=================================================================================================
    // Extensões adicionam novas funcionalidades para classes, estruturas ou enumerações já existentes
    // dando a possibilidade de estender seus métodos e propriedades sem que aconteça uma sobreposição
    // do original
    //=================================================================================================
    
    //--------------------------------
    //EXEMPLO 1
    //--------------------------------
    
    extension String
    {
        var maiusculo: String
        {
            return self.uppercased()
        }
        
        var minusculo: String
        {
            return self.lowercased()
        }
    }
    
    var teste = String()
    
    teste = "Extensões são legais !"
    
    print(teste.maiusculo)
    
    print(teste.minusculo)
    
    
    //--------------------------------
    //EXEMPLO 2
    //--------------------------------
    
    extension Double
    {
        var fahrenheitToCelsius: Double
        {
            return (self - 32.00) / 1.8000
        }
        
        var celsiusToFahrenheit: Double
        {
            return (self * 1.80) + 32.00
        }
    }
    
    let temp1Fahrenheit: Double = 212
    let temp2Celsius: Double = 100
    
    print(temp1Fahrenheit.fahrenheitToCelsius)
    
    print(temp2Celsius.celsiusToFahrenheit)

