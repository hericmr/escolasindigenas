# Escolas Indígenas

Um portal informativo interativo que mapeia e apresenta informações detalhadas sobre escolas indígenas no estado de São Paulo, Brasil. O projeto visa facilitar o acesso a dados educacionais e culturais dessas instituições, promovendo maior visibilidade e compreensão da educação indígena.

### Frontend
- **React 18** - Biblioteca principal para construção da interface
- **TailwindCSS** - Framework CSS utilitário para estilização
- **Lucide React** - Biblioteca de ícones
- **Leaflet** - Biblioteca para mapas interativos
- **Framer Motion** - Animações e transições
- **React Router** - Roteamento da aplicação

### Dados e APIs
- **Supabase** - Backend e banco de dados
- **GeoJSON** - Formato para dados geográficos
- **PapaParse** - Parser para arquivos CSV
- **React Markdown** - Renderização de conteúdo markdown

## Instalação

1. Clone o repositório:
```bash
git clone https://github.com/hericmr/escolasindigenas.git
cd escolasindigenas
```

2. Instale as dependências:
```bash
npm install
```

3. Inicie o servidor de desenvolvimento:
```bash
npm start
```

##  Estrutura do Projeto

```
src/
├── components/
│   ├── PainelInformacoes/           # Componente principal de informações
│   │   ├── components/              # Subcomponentes modulares
│   │   │   ├── EscolaInfo/         # Informações da escola
│   │   │   │   ├── BasicInfo.js    # Dados básicos
│   │   │   │   ├── PovosLinguas.js # Informações étnicas
│   │   │   │   ├── Ensino.js       # Dados educacionais
│   │   │   │   └── ...
│   │   │   ├── InfoSection.js      # Seção de informação reutilizável
│   │   │   ├── InfoItem.js         # Item de informação
│   │   │   └── ...
│   │   ├── hooks/                  # Hooks customizados
│   │   │   ├── usePainelVisibility.js
│   │   │   ├── useAudio.js
│   │   │   └── ...
│   │   └── index.js               # Componente principal
│   └── ...
├── data/                          # Dados estáticos
│   ├── escolas.csv
│   └── terras_indigenas.geojson
└── ...
```

## Componentes Principais

### PainelInformacoes
Componente central que gerencia a exibição de informações detalhadas sobre escolas e terras indígenas. Utiliza uma arquitetura modular com:

- **Componentes Modulares**: Separação clara de responsabilidades
- **Hooks Customizados**: Gerenciamento de estado e lógica reutilizável
- **Componentes Utilitários**: Elementos reutilizáveis como `InfoSection` e `InfoItem`

### Hooks Customizados
- `usePainelVisibility`: Controla visibilidade do painel
- `useAudio`: Gerencia recursos de áudio
- `useShare`: Funcionalidades de compartilhamento
- `useDynamicURL`: Gerenciamento de URLs dinâmicas
- `useClickOutside`: Detecção de cliques fora do componente
- `usePainelDimensions`: Responsividade e dimensões

## Estilização

O projeto utiliza TailwindCSS com configurações personalizadas:
- Sistema de cores verde para identidade visual
- Componentes responsivos
- Tipografia otimizada para leitura
- Animações suaves para interações

## 🧪 Testes

Execute os testes com:
```bash
npm test           # Executa testes
npm run test:watch # Modo watch
npm run test:coverage # Cobertura de testes
```


2. Configure o ambiente:
- Copie `.env.example` para `.env`
- Adicione suas credenciais do Supabase

3. Execute o projeto:
```bash
npm start
```

## Tecnologias

- React.js com Leaflet para mapas
- Tailwind CSS para estilização
- Supabase para backend

## Contato

Heric Rodrigues - [heric.moura@unifesp.br](mailto:heric.moura@unifesp.br)

---
Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
