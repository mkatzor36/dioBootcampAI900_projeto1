# Microsoft Azure AI Fundamentals

Bootcamp da DIO em parceria com a Microsoft, visando a preparação de profissionais para a certificação AI-900. 

# Projeto 1: Aprendizado de Máquina

Neste primeiro desafio de projeto, o objetivo é criar um modelo de predição para aluguéis de bicicletas, utilizando a ferramenta de aprendizado de máquina automatizado do Azure Machine Learning.

## Etapas do Projeto

### 1. Criando o Worskpace

Acesse o portal do Azure, utilizando uma conta Microsoft. Selecione a opção "Create a Resource" e acesse a ferramenta "Azure Machine Learning".
![Captura de Tela (133)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/e36c3278-0145-4ef1-ad30-0df5bd4478e7)

Entre com as seguintes configurações e selecione "Review + Create".
![Captura de Tela (134)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/dfdaf18f-99b7-440b-82cd-fc1c9ac41a1a)

Ao concluir o 'deployment', clique em "Go to Resource". Depois, clique em "Launch Studio".
![Captura de Tela (136)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/4bcca6cd-4c62-4c35-ad07-df6aab6296ab)
![Captura de Tela (137)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/3eda8895-399e-45e5-bd2d-f0138c9e895d)

### 2. Treinando o Modelo

Ao abrir o ML Studio, selecione a opção "Automated ML", na barra de opções à esquerda. Em seguida, selecione "New Automated ML Job".
![Captura de Tela (138)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/14321f4e-657b-4217-aa2d-a407970efbc2)

Com isso, crie um novo pedido, inserindo os parâmetros conforme a documentação.
![Captura de Tela (140)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/87a86fbd-c2ba-419a-8690-d12d3d0dabe1)
![Captura de Tela (141)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/a18e7a05-ede7-46b1-9770-26768771d415)
![Captura de Tela (143)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/3819da47-2f4f-49c6-80f3-a708d8d10ea7)
![Captura de Tela (144)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/6308927a-e22a-4b0b-8db8-7b3c0a73e2fc)
![Captura de Tela (148)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/f5317e68-036f-4ff0-8d6d-335390b60a3b)

Uma vez que os dados estão carregados, selecione o dataset "bike-rentals" e clique em "Next".
![Captura de Tela (152)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/5b60ba64-fc44-4872-bd53-04c5dd9e6211)

Em "Task Settings", insira as configurações conforme a documentação.
![Captura de Tela (154)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/c047244d-deca-4b80-a9b8-d742d8e0d7c0)
![Captura de Tela (155)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/ac7f1bcc-9b8f-480e-a8ad-15ebd7e6409a)
![Captura de Tela (156)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/e133251e-082e-4d1e-a3e2-67e1eab97346)

Em "Compute", selecione as seguintes opções:
![Captura de Tela (157)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/896fe620-ddf9-45c8-974a-1e3ea0d7a7f1)

Com isso, clique em "Submit training job".
![Captura de Tela (158)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/cca47d92-a7b4-4f2b-8843-3f8b3e4dc2f6)

### 3. Revisão e Teste

Espere o modelo ser computado, e seu status aparecer como "Completed". Tal tarefa leva de 10 a 15 minutos.
![Captura de Tela (160)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/00be07ea-d4aa-4eab-9d6d-2cd36f613f99)

Ao avaliar o melhor modelo, em "Best model summary", as métricas e os gráficos podem ser avaliados em "Metrics".
![Captura de Tela (161)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/510acabd-56ae-4ae3-b4fe-bf87ecbd54d6)
![Captura de Tela (162)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/c4bcb669-41c0-45d6-b076-4c68689e1c20)
![Captura de Tela (163)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/ec72c0aa-a0b3-46b9-9596-33d66101a8a7)

Em "Models", selecione o melhor modelo e clique em "Deploy" e, em seguida, em "Web service".
![Captura de Tela (164)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/2f6f6467-755f-46a6-93f2-ff4c664cfccd)

Espere o modelo carregar em "Endpoints", até que o "Deployment state" esteja como "Healthy". Tal tarefa leva em torno de 10 minutos.
![Captura de Tela (165)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/524e2f15-2f54-4020-acfc-66dd502f7e92)
![Captura de Tela (166)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/f1f31ca7-4f76-497e-93fb-7937fc93e016)

Vá em "Test" e insira os dados de input conforme a documentação e teste o modelo.
![Captura de Tela (168)](https://github.com/mkatzor36/dioBootcampAI900_projeto1-Azure-ML/assets/54877987/d7b29956-c5f2-4f27-9e60-28dfb46b8622)

## Referências

1. https://aka.ms/ai900-auto-ml;
2. https://aka.ms/ai900-azure-ai-services; 
