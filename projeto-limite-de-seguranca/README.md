LIMITE_SEGURANCA = 10000.0


def analisar_vendas(v1, v2, v3):
global LIMITE_SEGURANCA

    vendas = [v1, v2, v3]
    
    media = sum(vendas) / len(vendas)
    
    print("\n--- RESULTADO DA ANÁLISE ---")
    
    print(f"Média das vendas: R$ {media:.2f}")
   
    if media > LIMITE_SEGURANCA:
        print("⚠️ SISTEMA EM QUARENTENA ⚠️")
    for venda in vendas:
        if venda >= media * 5:
            print("🔎 REVISÃO MANUAL NECESSÁRIA")
            print(f"Venda suspeita detectada: R$ {venda:.2f}"
            resposta = input("Essa venda é legítima? (s/n): ").lower()
            if resposta == 's':
                novo_limite = float(input("Digite o novo LIMITE DE SEGURANÇA: "))
                LIMITE_SEGURANCA = novo_limite
                print(f"Novo limite definido: R$ {LIMITE_SEGURANCA:.2f}")
    print("\n--- TIPOS DE DADOS ---")
    print(f"v1: {v1} | tipo: {type(v1)}")
    print(f"v2: {v2} | tipo: {type(v2)}")
    print(f"v3: {v3} | tipo: {type(v3)}")
    print(f"media: {media} | tipo: {type(media)}")
    print(f"LIMITE_SEGURANCA: {LIMITE_SEGURANCA} | tipo: {type(LIMITE_SEGURANCA)}")


print("=== SISTEMA DE AUDITORIA DE VENDAS ===")

venda1 = float(input("Digite o valor da Venda 1: "))
venda2 = float(input("Digite o valor da Venda 2: "))
venda3 = float(input("Digite o valor da Venda 3: "))

analisar_vendas(venda1, venda2, venda3)
