# HaumeaNoSpiders

Transforme aranhas e aranhas da caverna em pequenos baús de madeira e continue explorando sem o visual clássico que causa desconforto.

O HaumeaNoSpiders é um pacote de recursos para Minecraft Java Edition voltado a jogadores com aversão ou medo de aranhas. Ele substitui texturas, olhos e sons; com suporte a modelos personalizados, também troca a silhueta da entidade por um mímico em formato de baú.

## O que muda

| Elemento | Resultado |
| --- | --- |
| Aranha | textura de mímico de madeira |
| Aranha da caverna | variação própria do mímico |
| Olhos | textura transparente, sem olhos brilhantes |
| Sons | eventos de ambiente, dano, passos e morte remapeados |
| Modelo | baú animado quando CEM está disponível |

O comportamento, a IA, a vida, o dano e a hitbox continuam sendo os da entidade original. Este é um pacote visual e sonoro; ele não remove aranhas do jogo.

## Duas formas de usar

### Somente o pacote de recursos

Funciona sem mods e troca texturas e sons. Como o Minecraft vanilla não aplica os arquivos CEM, a geometria básica da aranha pode continuar visível, apenas com a aparência de madeira.

### Com modelo de baú

Para esconder as pernas e usar o modelo completo:

- em Fabric, use [Entity Model Features (EMF)](https://modrinth.com/mod/entity-model-features) e, de preferência, [Entity Texture Features (ETF)](https://modrinth.com/mod/entitytexturefeatures);
- em uma instalação compatível, use OptiFine com suporte a Custom Entity Models.

Não misture OptiFine com uma instalação Fabric comum. Mantenha loader, mods e Minecraft na mesma versão.

## Instalação

1. Baixe o repositório em **Code → Download ZIP** ou faça o clone.
2. Garanta que `pack.mcmeta` e `assets/` estejam na raiz da pasta ou do ZIP final.
3. Copie para:

```text
%AppData%\.minecraft\resourcepacks\
```

4. No jogo, abra **Opções → Pacotes de recursos**.
5. Ative o HaumeaNoSpiders e deixe-o acima de outros pacotes que alterem aranhas.
6. Use `F3 + T` se precisar recarregar os recursos.

Para o modelo completo no Fabric, instale EMF e ETF em `.minecraft/mods/` antes de iniciar o jogo.

## Compatibilidade

O pacote foi usado principalmente com Fabric 1.20.2 e EMF/ETF. O `pack.mcmeta` declara uma faixa ampla em `supported_formats`, mas isso não garante que todas as versões futuras ou antigas interpretem texturas, sons e CEM da mesma maneira.

Se o Minecraft exibir um aviso de versão:

1. confirme se o pacote ainda carrega;
2. teste texturas, sons e as duas variantes de aranha;
3. use versões de EMF/ETF ou OptiFine compatíveis com o jogo.

## Estrutura

```text
HaumeaNoSpiders/
├── pack.mcmeta
├── pack.png
└── assets/minecraft/
    ├── sounds.json
    ├── sounds/mob/spider/
    ├── textures/entity/spider/
    ├── textures/entity/spider_eyes.png
    ├── cem/
    ├── emf/cem/
    └── optifine/cem/
```

As três cópias dos modelos `.jem` atendem caminhos reconhecidos por diferentes carregadores de CEM.

## Limitações

- A hitbox e a movimentação continuam sendo de aranha.
- Sem CEM, a troca de geometria não acontece.
- Outro pacote com prioridade maior pode sobrescrever os mesmos assets.
- Mudanças em EMF, OptiFine ou no formato dos pacotes podem exigir atualização.
- O pacote não altera nomes, drops, spawn ou mecânicas.

## Contribuição

Relate a versão do Minecraft, o carregador, a versão de EMF/ETF ou OptiFine e quais partes falharam: textura, som ou modelo. Pull requests devem manter as duas entidades e os caminhos CEM equivalentes.

## Créditos e direitos

HaumeaNoSpiders é um projeto independente e não é afiliado à Mojang ou à Microsoft. Minecraft, sua marca e seus assets pertencem aos respectivos titulares.

## Licença

O código e os arquivos próprios do projeto são distribuídos sob a [Licença MIT](LICENSE). Essa licença não concede direitos sobre conteúdo ou marcas de terceiros.
