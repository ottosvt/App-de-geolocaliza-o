Onde estou

Aplicativo mobile em React Native, desenvolvido no Expo Snack, que usa a geolocalização do dispositivo para mostrar onde o usuário está e registrar os lugares visitados.

Trabalho prático da disciplina de Desenvolvimento Mobile, com o professor Dionésio.

Aluno: Othon Henrique
Turma: 4p Noite (Uninassau Olinda)
Snack:https://snack.expo.dev/@othonsav/geolock
O que o app faz
Pede permissão de localização e mostra a latitude, a longitude e o endereço atuais.
Permite salvar o local como um check-in.
Lista os check-ins salvos, com data e hora, e permite excluí-los.
Se o usuário negar a permissão, mostra uma mensagem explicativa e um atalho para os Ajustes, sem apresentar erro.
Telas
Onde estou: obtém a localização e salva o check-in.
Check-ins: mostra a lista dos lugares salvos.

A navegação entre as telas usa @react-navigation/native-stack. O visual é inspirado no iOS: título grande, listas em cartões arredondados e azul do sistema como cor de destaque.

Tecnologias
React Native com Expo (Snack)
expo-location
@react-navigation/native
@react-navigation/native-stack
react-native-screens
react-native-safe-area-context
Como executar
Abra o link do Snack acima.
Para testar no celular, instale o aplicativo Expo Go e leia o QR Code exibido no Snack.
Permita o acesso à localização quando o aplicativo pedir.

Também é possível usar a prévia Web do Snack. Nela, o endereço pode aparecer como "Endereço não disponível", pois o navegador não faz essa conversão; no celular, o endereço costuma aparecer.

Como rodar fora do Snack
bash
npx create-expo-app onde-estou
cd onde-estou
npx expo install expo-location @react-navigation/native @react-navigation/native-stack react-native-screens react-native-safe-area-context

Depois, substitua o conteúdo do App.js pelo código deste repositório e execute npx expo start.

Observações
Os check-ins ficam guardados apenas em memória: ao fechar o aplicativo, a lista é apagada.
