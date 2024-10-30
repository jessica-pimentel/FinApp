# FinApp

FinApp é um aplicativo Android criado para gerenciamento simples de transações financeiras, permitindo ao usuário cadastrar transações de crédito e débito e visualizar em um extrato. O projeto utiliza MultiActivity para navegar entre as telas de cadastro e extrato bancário, além de armazenar os dados localmente utilizando `SharedPreferences`.

## 📱 Funcionalidades

- **Cadastro de Transações**: Adicione transações de crédito ou débito com descrição e valor.
- **Exibição do Extrato**: Visualize todas as transações cadastradas em uma lista organizada por ordem de criação.
- **Armazenamento Local**: As transações são salvas no `SharedPreferences`, garantindo que os dados sejam mantidos mesmo após fechar o aplicativo.
- **Toast de Validação**: O app exibe uma mensagem de alerta caso os campos obrigatórios não estejam preenchidos.

## 🛠️ Tecnologias Utilizadas

- **Kotlin**: Linguagem de programação principal.
- **Android SDK**: APIs de UI e Android.
- **Multi-Activity**: Implementação de múltiplas `Activities` para separar as telas de Cadastro e Extrato Bancário.
- **SharedPreferences**: Utilizado para armazenamento local das transações, garantindo persistência de dados.
- **Toast Notifications**: Notificações rápidas para feedback de usuário, como mensagens de erro e sucesso.

## ⚙️ Como Funciona
- **RegisterActivity**: Permite que o usuário insira uma descrição, um valor e escolha entre uma transação de crédito ou débito. Ao salvar, o app verifica se todos os campos foram preenchidos e exibe um Toast em caso de dados faltantes. A transação é então salva no SharedPreferences, e o usuário retorna para a tela inicial.

- **BankStatementActivity**: Exibe uma lista de todas as transações salvas em SharedPreferences, apresentando-as na ordem em que foram criadas. Cada item da lista mostra o tipo de transação, descrição e valor formatado.

- **Navegação entre Activities**: O aplicativo utiliza Intents para navegar entre as Activities, promovendo uma experiência de uso clara e intuitiva.

## 🚀 Como Executar
- Clone este repositório.
- Abra o projeto no Android Studio.
- Compile e execute o aplicativo em um emulador ou dispositivo Android.
