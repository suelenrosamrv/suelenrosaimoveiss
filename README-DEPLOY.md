# SR Negócios Imobiliários - Guia de Deploy

## 📋 Sobre o Projeto

Este é um site moderno e responsivo para negócios imobiliários, desenvolvido com React, Tailwind CSS e componentes shadcn/ui. O site inclui:

- **Homepage** com hero banner e listagem de empreendimentos
- **Página Sobre Mim** com informações da corretora
- **Simuladores** de financiamento e calculadora de investimento
- **Design responsivo** para desktop e mobile
- **Paleta de cores sofisticada** com tons terrosos e verde escuro

## 🚀 Deploy no GitHub

### 1. Criar Repositório no GitHub

1. Acesse [GitHub](https://github.com) e faça login
2. Clique em "New repository"
3. Nome sugerido: `sr-imoveis-site`
4. Marque como "Public" ou "Private" conforme preferir
5. **NÃO** marque "Initialize with README"
6. Clique em "Create repository"

### 2. Fazer Upload do Código

#### Opção A: Via GitHub Web (Mais Fácil)

1. Baixe o arquivo `sr-imoveis-site-completo.tar.gz`
2. Extraia o conteúdo em seu computador
3. No GitHub, clique em "uploading an existing file"
4. Arraste todos os arquivos da pasta `sr-imoveis-site/` para o GitHub
5. Adicione uma mensagem de commit: "Initial commit - SR Imóveis Site"
6. Clique em "Commit changes"

#### Opção B: Via Git (Terminal)

```bash
# Extrair o arquivo baixado
tar -xzf sr-imoveis-site-completo.tar.gz
cd sr-imoveis-site

# Inicializar git
git init
git add .
git commit -m "Initial commit - SR Imóveis Site"

# Conectar ao repositório GitHub (substitua SEU_USUARIO pelo seu username)
git remote add origin https://github.com/SEU_USUARIO/sr-imoveis-site.git
git branch -M main
git push -u origin main
```

## 🌐 Deploy na Vercel

### 1. Conectar GitHub à Vercel

1. Acesse [Vercel](https://vercel.com)
2. Faça login com sua conta GitHub
3. Clique em "New Project"
4. Selecione o repositório `sr-imoveis-site`
5. Clique em "Import"

### 2. Configurar o Deploy

1. **Framework Preset**: Vite (será detectado automaticamente)
2. **Root Directory**: `./` (padrão)
3. **Build Command**: `npm run build` (padrão)
4. **Output Directory**: `dist` (padrão)
5. **Install Command**: `npm install` (padrão)

### 3. Variáveis de Ambiente (Opcional)

Se necessário, adicione variáveis de ambiente na seção "Environment Variables":
- Não há variáveis específicas necessárias para este projeto

### 4. Finalizar Deploy

1. Clique em "Deploy"
2. Aguarde o build (aproximadamente 2-3 minutos)
3. Seu site estará disponível em uma URL como: `https://sr-imoveis-site-xxx.vercel.app`

## 🔧 Configurações Adicionais

### Domínio Personalizado (Opcional)

1. Na dashboard da Vercel, vá para o projeto
2. Clique em "Settings" > "Domains"
3. Adicione seu domínio personalizado (ex: `suelenrosaimoveis.com.br`)
4. Configure os DNS conforme instruções da Vercel

### Analytics (Opcional)

1. Na dashboard da Vercel, vá para "Analytics"
2. Ative o Vercel Analytics para monitorar visitantes
3. Dados aparecerão automaticamente no dashboard

## 📱 Funcionalidades do Site

### Navegação
- **Início**: Homepage com empreendimentos
- **Sobre Mim**: Informações da corretora Suelen Rosa
- **Oportunidades**: Redireciona para seção de empreendimentos
- **Simuladores**: Ferramentas de cálculo financeiro

### Simuladores Inclusos

#### 1. Simulador de Financiamento
- Valor do imóvel (R$ 200.000 - R$ 2.000.000)
- Entrada (0% - 80% do valor)
- Taxa de juros (6% - 15% a.a.)
- Prazo (10 - 35 anos)
- **Resultado**: Parcela mensal calculada

#### 2. Calculadora de Investimento
- Valor do investimento
- Valor do imóvel
- Aluguel mensal esperado
- Taxa de valorização anual
- Período de investimento
- **Resultado**: ROI projetado e retorno total

### Empreendimentos Cadastrados

1. **Sensia Aurora** (Em Construção)
   - 58m² a 60m²
   - Valorização: 8% a.a.
   - Yield: 14% a.a.
   - Entrega: Dezembro 2026

2. **Residencial Lancelot** (Lançamento)
   - 44m² a 46m²
   - Valorização: 7% a.a.
   - Yield: 13% a.a.

3. **Residencial La Roche** (Lançamento)
   - 45m² a 50m²
   - Valorização: 7% a.a.
   - Yield: 12% a.a.

4. **Lake Dali** (Lançamento)
   - 1 e 2 quartos
   - Valorização: 6% a.a.
   - Yield: 11% a.a.

5. **Lake Da Vinci** (100% Vendido)
   - Exemplo de sucesso de vendas

6. **Lake Picasso** (100% Vendido)
   - Exemplo de sucesso de vendas

## 🎨 Personalização

### Cores do Site
- **Verde Escuro**: `#1B4332` (Botões principais)
- **Marrom Terroso**: `#8B4513` (Elementos secundários)
- **Branco**: `#FFFFFF` (Fundo)
- **Preto**: `#000000` (Textos)

### Modificar Conteúdo

Para alterar informações do site, edite o arquivo `src/App.jsx`:

1. **Dados da corretora**: Seção "Sobre Mim"
2. **Empreendimentos**: Array de propriedades na seção home
3. **Contatos**: Seção footer
4. **Valores dos simuladores**: Ranges nos componentes

### Adicionar Novos Empreendimentos

No arquivo `src/App.jsx`, adicione novos cards seguindo o padrão:

```jsx
<div className="property-card bg-card rounded-lg overflow-hidden border border-border">
  {/* Conteúdo do card */}
</div>
```

## 📞 Suporte

Para dúvidas sobre o deploy ou personalização:

- **Email**: suelen_rosa@gmail.com
- **Telefone**: (43) 98870-7994
- **WhatsApp**: (43) 98842-3605

## 🔄 Atualizações Futuras

Para atualizar o site:

1. Faça as alterações no código local
2. Commit e push para o GitHub
3. A Vercel fará deploy automático das mudanças
4. Site atualizado em 1-2 minutos

---

**Desenvolvido com ❤️ para SR Negócios Imobiliários**

