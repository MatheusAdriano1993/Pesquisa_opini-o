# Pesquisa de opinião para uma determinada loja

Segue abaixo o codigo com a programação em Python, para executar a programação basta copiar o codigo e abrir um leitor Python para executar a pesquisa.



  # Inicialização dos contadores para as respostas exigidas
qtd_excelente = 0
qtd_bom = 0
qtd_ruim = 0

print("PESQUISA DE ATENDIMENTO AO CLIENTE TUDOWEB")

# Definindo a quantidade de entrevistados para o teste
TOTAL_ENTREVISTADOS = 10

# Estrutura de repetição para coletar os dados
for i in range(1, TOTAL_ENTREVISTADOS + 1):
  print(f"Entrevistado {i} de {TOTAL_ENTREVISTADOS}")

  # Coleta de dados básicos
  nome = input("Digite o nome do entrevistado: ")
  idade = int(input("Digite a idade do entrevistado: "))

  # Apresentação das opções de opinião
  print("Opinião sobre o atendimento prestado:")
  print("  [1] EXCELENTE")
  print("  [2] BOM")
  print("  [3] RUIM")

  # Coleta da opinião
  opiniao = int(input("Digite o código correspondente (1, 2 ou 3): "))

  # Validação para garantir que o usuário digite apenas opções válidas
  while opiniao not in [1, 2, 3]:
    print("Opção inválida! Por favor, digite 1, 2 ou 3.")
    opiniao = int(input("Digite o código correspondente (1, 2 ou 3): "))

  # Estrutura de decisão para contabilizar as respostas
  if opiniao == 1:
    qtd_excelente += 1
  elif opiniao == 2:
    qtd_bom += 1
  elif opiniao ==3:
    qtd_ruim += 1

# Exibição dos resultados finais consolidados
print("RESULTADO FINAL DA PESQUISA")
print(f"a) Quantidade de respostas 'EXCELENTE': {qtd_excelente}")
print(f"b) Quantidade de respostas 'BOM': {qtd_bom}")
print(f"c) Quantidade de respostas 'RUIM': {qtd_ruim}")
