# 📱 Meu Aplicativo Flutter

Aplicativo desenvolvido utilizando **Flutter** e a linguagem **Dart**, com uma tela inicial que apresenta as principais funcionalidades disponíveis no projeto.

A tela `Home` funciona como um menu principal, permitindo ao usuário acessar diferentes recursos por meio de botões de navegação.

## 🚀 Funcionalidades

O aplicativo possui atualmente as seguintes funcionalidades:

- 🏠 **Tela inicial**
- 📍 **Localização**
- 📷 **Câmera e Galeria**
- 🧭 Navegação entre telas utilizando rotas nomeadas
- 📱 Interface adaptada para dispositivos móveis

## 🖥️ Tela Home

A tela inicial apresenta:

- Barra superior com o título **"Meu Aplicativo"**;
- Ícone representando um dispositivo móvel;
- Mensagem de boas-vindas;
- Descrição das funcionalidades;
- Botão para acessar a tela de **Localização**;
- Botão para acessar a tela de **Câmera e Galeria**.

## 🧭 Navegação

A navegação é realizada utilizando o `Navigator.pushNamed()` do Flutter.

### Localização

Ao clicar no botão **Localização**, o aplicativo direciona o usuário para:

```dart
Navigator.pushNamed(
  context,
  '/localizacao',
);
```

### Câmera e Galeria

Ao clicar no botão **Câmera e Galeria**, o aplicativo direciona o usuário para:

```dart
Navigator.pushNamed(
  context,
  '/camera',
);
```

As rotas precisam estar configuradas no arquivo principal do aplicativo, normalmente no `main.dart`.

Exemplo:

```dart
routes: {
  '/localizacao': (context) => const Localizacao(),
  '/camera': (context) => const Camera(),
},
```

## 🛠️ Tecnologias utilizadas

- **Flutter**
- **Dart**
- **Material Design**
- `Scaffold`
- `AppBar`
- `Column`
- `Padding`
- `Icon`
- `Text`
- `ElevatedButton.icon`
- `Navigator.pushNamed`

## 📂 Estrutura do projeto

Uma possível organização do projeto é:

```text
lib/
├── main.dart
├── home.dart
├── localizacao.dart
└── camera.dart
```

### `main.dart`

Arquivo responsável pelo ponto de entrada do aplicativo e pela configuração das rotas.

### `home.dart`

Contém a tela principal do aplicativo e os botões de acesso às funcionalidades.

### `localizacao.dart`

Tela destinada à funcionalidade de localização geográfica, utilizando informações de latitude e longitude.

### `camera.dart`

Tela destinada às funcionalidades relacionadas à câmera e à galeria do dispositivo.

## 🎨 Interface

A interface foi construída utilizando componentes do **Material Design** disponibilizados pelo Flutter.

Os botões utilizam `ElevatedButton.icon`, combinando ícones e textos para facilitar a identificação das funcionalidades.

Exemplo:

```dart
ElevatedButton.icon(
  onPressed: () {
    Navigator.pushNamed(
      context,
      '/camera',
    );
  },
  icon: const Icon(Icons.camera_alt),
  label: const Text(
    'Câmera e Galeria',
  ),
)
```

## ▶️ Como executar o projeto

### 1. Instalar o Flutter

Certifique-se de que o Flutter esteja instalado e configurado no computador.

Verifique a instalação utilizando:

```bash
flutter doctor
```

### 2. Clonar o projeto

```bash
git clone URL_DO_SEU_REPOSITORIO
```

### 3. Entrar na pasta

```bash
cd nome_do_projeto
```

### 4. Instalar as dependências

```bash
flutter pub get
```

### 5. Executar o aplicativo

```bash
flutter run
```

O aplicativo poderá ser executado em um dispositivo físico ou em um emulador Android/iOS.

## 📌 Objetivo do projeto

O objetivo do projeto é desenvolver um aplicativo mobile utilizando **Flutter e Dart**, aplicando conceitos de construção de interfaces, navegação entre telas e utilização de recursos do dispositivo.

A tela `Home` serve como ponto central para que o usuário possa acessar as diferentes funcionalidades desenvolvidas no aplicativo.

## 🔮 Possíveis melhorias

O projeto pode ser expandido com novas funcionalidades, como:

- 📍 Exibição da localização atual;
- 📷 Captura de fotos pela câmera;
- 🖼️ Seleção de imagens da galeria;
- 🗺️ Exibição da localização em um mapa;
- 🎨 Aplicação de uma paleta de cores personalizada;
- ✨ Animações entre as telas;
- 💾 Armazenamento de informações;
- 🔙 Botões de retorno e navegação mais dinâmica.

## 👩‍💻 Autora

**Thais Costa Patto Souza**

Projeto desenvolvido para fins acadêmicos utilizando **Flutter e Dart**.
