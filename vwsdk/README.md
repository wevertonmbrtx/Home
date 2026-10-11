# vwsdk

Projeto Android (Kotlin) de acesso remoto ao celular Samsung com tela quebrada do Weverton.
Branch criada para receber o código-fonte quando ele tiver acesso ao computador de novo.

## Próximos passos

1. Subir o projeto Gradle completo (código Kotlin, `AndroidManifest.xml`, `build.gradle*`,
   `gradle/`, etc.) dentro desta pasta `vwsdk/`.
2. Remover o `BroadcastReceiver` de código secreto do discador
   (`android.provider.Telephony.SECRET_CODE` no manifest) e o trecho correspondente no Kotlin,
   já que a ativação será direta por um botão no app, sem gatilho escondido.
3. Recompilar (`./gradlew assembleDebug`) e reinstalar com `adb install -r`, desinstalando
   qualquer versão anterior com assinatura diferente (`adb uninstall com.vwsdk.app`) se
   necessário.

## Pacote

- `applicationId`: `com.vwsdk.app`
- `minSdk`: 26 · `targetSdk`: 34
