# 📱 Leitor de QR por Arquivo + Hash


Este é um aplicativo web simples e moderno que permite **ler um QR Code a partir de uma imagem** e gerar automaticamente o **código hash (SHA-256, SHA-1 ou SHA-512)** do conteúdo decodificado.


---


## 🚀 Funcionalidades


- 📸 **Leitura de QR Code via arquivo** (PNG, JPG, etc.)
- 🔐 **Geração automática de hash** (SHA-256 por padrão)
- ⚙️ **Opção para escolher o algoritmo** (SHA-1, SHA-256, SHA-512)
- 💾 **Baixar o resultado em JSON** (contendo texto, hash e metadados)
- 🎨 Interface moderna, responsiva e sem dependências pesadas


---


## 🧰 Tecnologias utilizadas


- **HTML5 / CSS3 / JavaScript (ES6)**
- **[jsQR](https://github.com/cozmo/jsQR)** — biblioteca para leitura de QR Codes
- **Web Crypto API** — para geração de hashes de forma segura


---


## 🖥️ Como usar


1. Faça o download ou clone este repositório:
```bash
git clone https://github.com/seuusuario/leitor-qr-hash.git
cd leitor-qr-hash
```
2. Abra o arquivo `index.html` em um navegador moderno (Chrome, Edge, Firefox, etc.)
3. Selecione uma imagem contendo um QR Code
4. Clique em **“Ler e gerar hash”**
5. O app exibirá o texto decodificado e o hash correspondente


---


## 📄 Estrutura do projeto


```bash
📦 leitor-qr-hash
┣ 📜 index.html # Código principal do app (frontend)
┗ 📜 README.md # Documentação do projeto
```


---


## 📦 Resultado em JSON


Ao clicar em **“Baixar resultado”**, será gerado um arquivo `.json` contendo:


```json
{
"timestamp": "2025-11-12T22:00:00.000Z",
"algorithm": "SHA-256",
"decodedText": "https://exemplo.com",
"hash": "a8f1b3c9...",
"filename": "qrcode.png"
}
```


---


## 🧠 Observações


- Certifique-se de usar imagens nítidas e bem iluminadas para melhores resultados.
- O cálculo de hash é feito totalmente **no navegador**, sem enviar dados para servidores.
