# Analisando-Imagem-AzureVisionStudio

# Analisando uma imagem com o Azure Vision e recebendo o retorno em JSON
# Primeiro, acesse o Azure Portal e crie um recurso do tipo Cognitive Services ou Computer Vision. Durante a criação, defina nome, região e plano de preço. Quando o recurso estiver pronto, copie o Endpoint e a Key, pois serão necessários para autenticação.
![parte 4](https://github.com/user-attachments/assets/b7ad4c0a-9f75-4a1c-8043-f718107fb0cf)

# Depois, vá para Vision Studio e faça login com sua conta Azure. Selecione o recurso que você criou para vincular o serviço. No Vision Studio, escolha a funcionalidade desejada, como Detect faces para detecção facial, Read text para OCR ou Analyze images para descrição geral. Clique em Try it out para iniciar.
# Em seguida, faça o upload da imagem clicando em Browse for a file e aguarde o processamento. O Vision Studio exibirá os resultados na tela, incluindo caixas delimitadoras sobre os rostos detectados, atributos estimados como idade, gênero e pose da cabeça, além do nível de confiança da detecção.
![parte 5](https://github.com/user-attachments/assets/58d997a4-b883-4cbb-8906-11d6fc9d7bac)

Retorno
# JSON
{
  "modelVersion": "2023-04-15",
  "metadata": {
    "width": 520,
    "height": 693,
    "format": "Jpeg"
  },
  "faces": [
    {
      "boundingBox": {
        "x": 150,
        "y": 180,
        "width": 220,
        "height": 220
      },
      "confidence": 0.99,
      "attributes": {
        "age": 30,
        "gender": "male",
        "headPose": {
          "roll": 0.0,
          "yaw": 0.0,
          "pitch": 0.0
        }
      }
    }
  ]
}
