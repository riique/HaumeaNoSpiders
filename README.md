# HaumeaNoSpiders

Resource pack para Minecraft que troca **aranhas** e **aranhas da caverna** por **mímicos de baú de madeira** — visual calmo, sem carinha e sem o visual clássico de aranha.

Ideal para quem tem aversão a aranhas e quer continuar jogando sem o susto visual (e sonoro) delas.

---

## O que o pack faz

| Conteúdo | Mudança |
|----------|---------|
| **Aranha** | Textura de baú de madeira (mímico) |
| **Aranha da caverna** | Mesma madeira de baú |
| **Olhos / boca** | Removidos — só tábuas e trava dourada |
| **Sons** | Sons de **slime** (ambiente, passos, dano, morte) |
| **Modelo 3D de baú** *(opcional)* | Com EMF ou OptiFine (CEM) |

> **Limitação do vanilla:** sem EMF/OptiFine o Minecraft **não troca o modelo** da entidade. O formato base ainda é o da aranha (perninhas), mas a textura é toda de baú. Com **EMF** (Fabric) ou **OptiFine**, o pack usa modelos CEM para um visual mais de baú.

---

## Requisitos

### Mínimo (qualquer versão, sem mods)

- Minecraft Java Edition  
- Este resource pack ativado  

Funciona **só com resource pack**: texturas + sons.

### Recomendado (modelo de baú completo)

**Fabric** (ex.: 1.20.2):

1. [Fabric API](https://modrinth.com/mod/fabric-api)  
2. [Entity Model Features (EMF)](https://modrinth.com/mod/entity-model-features)  
3. [Entity Texture Features (ETF)](https://modrinth.com/mod/entitytexturefeatures) *(recomendado junto com EMF)*  

**Ou** OptiFine na versão do jogo (launcher oficial / Forge — **não** misture OptiFine com Fabric).

> No Fabric, use **EMF + ETF**, não OptiFine.

---

## Como instalar

### 1. Baixar o pack

- Clone o repositório, **ou**  
- Em GitHub: **Code → Download ZIP**, depois extraia a pasta do pack  

A pasta do pack deve conter `pack.mcmeta` e a pasta `assets` na raiz (não uma pasta “extra” em volta se você zipar de novo).

### 2. Colocar em Resource Packs

Copie a pasta do pack para:

```text
.minecraft/resourcepacks/
```

No Windows, o caminho costuma ser:

```text
%AppData%\.minecraft\resourcepacks\
```

### 3. Ativar no jogo

1. Abra o Minecraft  
2. **Opções → Resource Packs**  
3. Mova **HaumeaNoSpiders** (ou o nome da pasta) para a lista da **direita**  
4. Deixe-o **no topo** se usar outros packs  
5. Confirme e entre no mundo  

Se algo não atualizar: **F3 + T** (recarrega recursos) ou reinicie o jogo.

### 4. (Opcional) Mods no Fabric

Coloque EMF e ETF em `.minecraft/mods/`, na **mesma versão** do Minecraft (ex.: 1.20.2), com Fabric Loader + Fabric API.

---

## Estrutura do pack

```text
HaumeaNoSpiders/
├── pack.mcmeta
├── pack.png
├── README.md
└── assets/minecraft/
    ├── sounds.json
    ├── sounds/mob/spider/          # áudios (slime)
    ├── textures/entity/spider/     # texturas mímico
    ├── textures/entity/spider_eyes.png
    ├── optifine/cem/               # modelos CEM (EMF/OptiFine)
    ├── emf/cem/
    └── cem/
```

---

## Compatibilidade

- **Texturas e sons:** ampla (Java Edition com resource packs modernos)  
- **`pack_format` / `supported_formats`:** pensado para cobrir várias versões  
- **CEM (`.jem`):** OptiFine e EMF  

Testado principalmente no fluxo **Fabric 1.20.2** com EMF/ETF.

---

## Notas

- A **hitbox** continua a da aranha (limite de resource pack).  
- Aranha e aranha da caverna usam a **mesma ideia visual** (madeira de baú).  
- Sons oficiais de slime do jogo, remapeados para os eventos da aranha.  

---

## Créditos

- Pack original: **HaumeaNoSpiders**  
- Inspiração de conceito: packs de “arachnophobia” / mímicos no lugar de aranhas  
- Sons de slime: assets vanilla do Minecraft (Mojang)  

---

## Licença

Uso livre para jogar e modificar.  
**Minecraft** e seus assets oficiais pertencem à Mojang/Microsoft. Este pack não é afiliado à Mojang.
