# Payface App SDK iOS

Payface App SDK para IOS fornece um SDK nativo para integração com o Payface App. Você pode usar o SDK para integrar o Payface nos seus aplicativos personalizados.

Para notas de lançamento, consulte [CHANGELOG.md](https://github.com/PayfaceBrasil/payface-app-integration-sdk-ios/blob/master/CHANGELOG.md).

## Requisitos

**Versão**
Target 13


## Como Usar

**Configuração**

Adicionar permissão de utilização da camera(Privacy - Camera Usage Description) no arquivo Info.plist

No **Project Navigator** selecione a raiz do projeto, abrirá a painel de configuração. Selecione a aba **General**. Procure por **Framework, Libraries, and Embedded Content**. Adicione o framework da **hybrid.framework**.

**Integração no código:**

No *ViewController* 

```
import hybrid

.
.
.
// Código que abre a ViewController do Payface
present(HybridViewController(partner: "partner", cpf: "cpf", name: "nome", cellphone: "celular"), animated: true, completion: nil)
.
.

```
## Serviços Suportados

Acesso ao app web Payface com utilização da câmera nativa IOS. 

Existem dois framework no repositório: um caso você esteja compilando seu projeto no device simulado e outro para device real. O referente ao device simulado, a câmera não irá funcionar.

## Relatar um Problema

Se você encontrar um problema com o Payface App SDK iOS, pesquise as [issues existentes](https://github.com/PayfaceBrasil/payface-app-integration-sdk-ios/issues)
e tente se certificar de que seu problema ainda não existe antes de [abrir uma nova issue](https://github.com/PayfaceBrasil/payface-app-integration-sdk-ios/issues/new). É útil incluir a versão do SDK, ambiente e sistema operacional que você está usando. Inclua também um stack trace e os passos necessários para reproduzir o cenário.

## Licença

Consulte [LICENSE.md](https://github.com/PayfaceBrasil/payface-app-integration-sdk-ios/blob/master/LICENSE.md) e [NOTICE.md](https://github.com/PayfaceBrasil/payface-app-integration-sdk-ios/blob/master/NOTICE.md) para mais informações.
