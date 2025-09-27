
# 🔢 Classificação de Dígitos - MNIST

<a href="https://colab.research.google.com/github/JoseTayllan/Mnist/blob/main/Mnist.ipynb" target="_parent">
    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

## 📚 Informações
- **Curso:** GTI  
- **Disciplina:** Inteligência Artificial Aplicada  
- **Professor:** Jonas Augusto Kunzler  
- **Aluno:** José Tayllan Pinto Almeida  
- **Data:** 2025  

---

## 📖 Descrição
Este projeto implementa uma **Rede Neural Artificial (RNA)** para classificação da base de dados **MNIST**  
(dígitos escritos à mão, de 0 a 9).  
O modelo foi construído utilizando **TensorFlow/Keras** e avalia sua acurácia no conjunto de teste.

---

## ⚙️ Estrutura do Notebook
1. Importação de bibliotecas: `tensorflow`, `numpy`, `matplotlib`  
2. Carregamento da base **MNIST** (60.000 imagens treino, 10.000 teste)  
3. Pré-processamento: normalização dos pixels (0–255 → 0–1)  
4. Construção do modelo com `Sequential`:
   - `Flatten` (28x28 → vetor)
   - Camadas densas ocultas `[128, 64]` neurônios, ativação `relu`
   - Camada de saída `Dense(10, softmax)`
5. Compilação do modelo com **Adam optimizer** e `sparse_categorical_crossentropy`  
6. Treinamento da rede neural  
7. Avaliação do modelo no conjunto de teste  
8. Visualização de previsões com **matplotlib**  

---

## 📊 Exemplos de Resultados
O notebook gera:
- Gráficos de imagens do dataset com suas previsões  
- Métricas de avaliação (acurácia, perda)  
- Evolução do aprendizado durante o treinamento  

---

## ▶️ Como Executar
1. Clone este repositório  
2. Abra o notebook no Jupyter ou Google Colab  
3. Execute as células em ordem  

```bash
pip install tensorflow matplotlib numpy
```

---

## 🌱 Melhorias Futuras
- Testar diferentes funções de ativação (`sigmoid`, `tanh`)  
- Adicionar **Dropout** para reduzir overfitting  
- Implementar **CNN (Convolutional Neural Network)** para melhor acurácia  
- Exportar o modelo treinado para uso em aplicações externas  

---

📍 **Responsável:** José Tayllan Pinto Almeida
