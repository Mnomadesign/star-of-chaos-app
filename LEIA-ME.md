# Star of Chaos — pacote PWA

O pacote contém `index.html`, manifesto, ícones e service worker. Quando servido num endereço HTTPS, pode ser instalado no Android e armazena os arquivos do app para abrir offline depois da primeira visita.

## Importante

Abrir `index.html` diretamente de um ZIP/gerenciador de arquivos **não instala a PWA**: instalação e service worker exigem um site servido em HTTPS (ou localhost). A versão online está publicada em https://mnomadesign.github.io/star-of-chaos-app/. Abra esse mesmo endereço no Chrome Android; para atualizar uma instalação existente, basta abrir o app conectado à internet e aguardar a atualização. O service worker guarda os arquivos principais para acesso offline após o primeiro carregamento.

Os dados pessoais ficam no armazenamento local do navegador/aparelho, sem sincronização automática. Faça exportações de backup regularmente. O app não sincroniza automaticamente entre dispositivos.

## Home e lançamentos

- Painel inspirado no modelo descrito do Claude: saldo líquido em destaque, meta editável, 24 blocos estimados de R$ 50, resumo dos últimos 7 dias, missão e rotina essencial.
- Em Dinheiro, escolha entrada ou saída, categoria e valor; não é preciso escrever descrição. Há atalhos de valores rápidos. Os lançamentos entram nos totais de bruto, custos e líquido e podem ser excluídos com confirmação.
- Ganhos registrados por Uber/99 substituem os blocos estimados, evitando somar duas vezes. Lançamentos manuais positivos/negativos continuam sendo adicionados.
- Os dados da versão anterior com chave `central-vida-v1` são importados automaticamente para `star-of-chaos-v1` quando o novo app abre no mesmo navegador.

## Recursos

Rotina e modo dia difícil, Saúde, Trabalho, Dinheiro, Projetos, Pagamentos futuros, Calendário, Semana, Feed e backup JSON.

## Limites importantes

A agenda é interna ao app: ela não grava compromissos no Google Calendar nem em outro calendário do aparelho. Não cria notificações, não sincroniza entre dispositivos, não acessa banco, nem registra compromissos no calendário externo. Totais dependem dos valores digitados. Faça backup regularmente.
