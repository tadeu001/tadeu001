import random

# Simulando dados de produção agropecuária
class AgroData:
    def __init__(self):
        self.crops = ["Milho", "Soja", "Trigo", "Arroz", "Cana-de-açúcar"]
        self.production = {crop: random.randint(1000, 5000) for crop in self.crops}
        self.sustainable_practices = ["Uso de práticas de rotação de culturas", 
                                      "Agricultura de precisão", 
                                      "Cultivo orgânico", 
                                      "Uso de biopesticidas"]

    def display_data(self):
        print("Dados de Produção Agropecuária - 2025")
        print("---------------------------------------")
        for crop, amount in self.production.items():
            print(f"{crop}: {amount} toneladas")

    def suggest_practices(self):
        print("\nPráticas Sustentáveis Sugeridas:")
        for practice in self.sustainable_practices:
            print(f"- {practice}")


# Criando uma instância da classe AgroData
agro_data = AgroData()

# Exibindo dados
agro_data.display_data()
agro_data.suggest_practices()
