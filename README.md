# tabuada-poo

class Tabuada:
    def __init__(self, numero):
        self.numero = numero
        self._resultado = 0

    def soma(self):
        for i in range(1, 11):
            self._resultado = self.numero + i
            print(f"{self.numero} + {i} = {self._resultado}")

    def subtracao(self):
        for i in range(1, 11):
            self._resultado = self.numero - i
            print(f"{self.numero} - {i} = {self._resultado}")

    def multiplicacao(self):
        for i in range(1, 11):
            self._resultado = self.numero * i
            print(f"{self.numero} * {i} = {self._resultado}")

    def divisao(self):
        for i in range(1, 11):
            if i == 0:
                print("Não é possível dividir por zero.")
            else:
                self._resultado = self.numero / i
                print(f"{self.numero} / {i} = {self._resultado:.2f}")

numero = int(input("Digite um número: "))
tabuada = Tabuada(numero)

print("\nSoma:")
tabuada.soma()

print("\nSubtração:")
tabuada.subtracao()

print("\nMultiplicação:")
tabuada.multiplicacao()

print("\nDivisão:")
tabuada.divisao()
