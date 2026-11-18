# ORBITAL PULSE — Android nativo

![Ícone OP](app/src/main/res/mipmap-xxxhdpi/ic_launcher.png)

Jogo de reflexos com órbitas, obstáculos e orbes. Desenvolvido em **Kotlin com Android Canvas**, sem WebView e sem dependências de rede.

## Requisitos

- **Android mínimo:** 4.3 (API 18)
- **compileSdk / targetSdk:** 35
- **Android Gradle Plugin:** 8.6.1
- **Gradle:** 8.7
- **JDK:** 17
- **Kotlin:** 1.9.25

## Jogabilidade

- Deslizar para cima/baixo: muda de órbita.
- Toque simples: inverte o sentido **uma única vez por troca de anel**.
- Cada inversão extra válida aumenta multiplicativamente a velocidade em **1,1x**.
- Pontuação de 1 em 1 ao coletar orbes.
- Começa com 2 anéis; libera mais 1 a cada 2 pontos, até 6 anéis.
- Velocidade-base de 60% a 100% nos primeiros 10 pontos. A partir de 25 pontos, cresce 2 pontos percentuais a cada 3 pontos adicionais, além dos bônus de inversão.
- Interface responsiva para retrato, paisagem e telas 1:1.
- 7 opções de idioma com bandeiras desenhadas em Canvas, inclusive em Android 4.3.

## Abrir e gerar APK

1. Abra a pasta deste repositório no **Android Studio**.
2. Configure **Gradle JDK 17** e instale o **Android SDK 35** quando solicitado.
3. Sincronize o Gradle.
4. Use **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. O APK de desenvolvimento ficará em `app/build/outputs/apk/debug/app-debug.apk`.

**Atenção:** esta distribuição do código-fonte **não inclui o arquivo binário `gradle-wrapper.jar` nem os scripts `gradlew` e `gradlew.bat`**. Se você já tem uma versão do projeto que compila no Android Studio, copie dela `gradle/wrapper/gradle-wrapper.jar`, `gradlew` e `gradlew.bat`. Se estiver usando uma instalação local do Gradle 8.7, pode gerar o wrapper com `gradle wrapper --gradle-version 8.7`. O arquivo `gradle-wrapper.properties` com a versão correta já foi incluído.

## Publicação no GitHub

Este repositório hospeda **o código-fonte do aplicativo Android**, não uma versão executável pelo navegador. O GitHub Pages não executa aplicativos Kotlin/Android nativos. Para distribuir o jogo, gere o APK e publique-o como anexo de uma **Release** do GitHub.

## Licença

Nenhuma licença de reutilização de código foi definida neste pacote. O proprietário pode adicionar uma licença mais tarde, conforme desejar.
