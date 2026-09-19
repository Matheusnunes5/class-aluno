class Aluno:
    def __init__(self, nome, matricula, nota1, nota2, nota3, nota4, nota5):
        self.nome = nome
        self.matricula = matricula
        self.nota1 = nota1
        self.nota2 = nota2
        self.nota3 = nota3
        self.nota4 = nota4
        self.nota5 = nota5
    def calcular_media(self):
        soma = self.nota1 + self.nota2 + self.nota3 + self.nota4 + self.nota5
        self.media = soma/5

        return self.media
    

    def verificar_situacao(self):
      media = self.calcular_media()
      if media >= 7.0:
          print(f" O aluno {self.nome} foi aprovado")
      else:
        print(f" O aluno {self.nome} foi reprovado")
        

"""Criando alguns objetos que tem origem da classe aluno"""
al1=Aluno("Divo", "111", 9,6,7,8,9)
al2=Aluno("Maria", "222", 6,8,9,7,6)

al1.verificar_situacao()
