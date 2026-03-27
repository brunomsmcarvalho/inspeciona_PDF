📄 PDF Form Reader (JavaScript)

Este script em JavaScript permite ler um ficheiro PDF que se encontra na mesma pasta e listar todos os campos de formulário existentes no documento.

É útil para:

Inspecionar PDFs com formulários
Obter nomes de campos para automação
Preparar preenchimento automático de PDFs
🚀 Tecnologias utilizadas
Node.js
pdf-lib
fs (módulo nativo do Node.js)
📂 Estrutura esperada

Certifica-te de que tens o seguinte:

'/project-folder
│
├── script.js
├── DocumentoReforçoPPRSGFStoik.pdf
└── package.json'

⚙️ Instalação
Clona o repositório ou copia os ficheiros:
git clone <teu-repositorio>
cd <nome-da-pasta>
Instala as dependências:
npm install pdf-lib
▶️ Como usar
Coloca o ficheiro PDF na mesma pasta do script
Confirma que o nome do ficheiro no código corresponde ao PDF:
const pdfBytes = fs.readFileSync('DocumentoReforçoPPRSGFStoik.pdf');
Executa o script:
node script.js
📌 Código

No código basta alterar o campo:
fs.readFileSync('NOME_DO_PDF.pdf');

Pelo nome do seu pdf

📊 Output esperado

O script irá imprimir no terminal algo como:

nome TextField
email TextField
data DateField

Onde:

nome do campo → identificação no PDF
tipo do campo → tipo de input (TextField, CheckBox, etc.)
⚠️ Notas importantes
O PDF deve conter campos de formulário interactivos
Certifica-te que estás a usar Node.js com suporte para import (ou activa "type": "module" no package.json)
Se necessário, podes adaptar o script para preencher os campos automaticamente
