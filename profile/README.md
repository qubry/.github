<p align="center">
  <a href="https://qubry.dev"><img src="https://qubry.dev/assets/img/qubry-mark.svg?171126202806" width="72" alt="Qubry"></a>
</p>

<h1 align="center">Build beyond code.</h1>

<p align="center">
  Ferramentas nativas para quem constrói software com IA:<br>
  editor, orquestração de agentes, terminal, banco de dados e o consumo das suas IAs à vista.<br><br>
  <a href="https://qubry.dev"><b>qubry.dev</b></a> ·
  <a href="https://qubry.dev/docs/">Documentação</a> ·
  <a href="https://x.com/Qubrydev">X</a> ·
  <a href="https://www.instagram.com/qubrydev/">Instagram</a>
</p>

> [!IMPORTANT]
> **Todas as ferramentas Qubry estão em beta fechado, só para convidados.**
> Studio, Agents, Terminal, CountCode e DB ainda não têm download público. Quem recebeu convite tem acesso aos instaladores e às atualizações; para os demais, os apps chegam aqui e em [qubry.dev](https://qubry.dev) quando o beta abrir.

<p align="center">
  <img src="https://qubry.dev/assets/img/studio.jpg" width="860" alt="Janela de agentes do Qubry Studio">
</p>

## Produtos

<table>
  <tr>
    <td width="50%" valign="top">
      <img src="https://qubry.dev/assets/img/studio-icon.png?171126202806" width="48" alt="Ícone do Qubry Studio"><br>
      <b><a href="https://qubry.dev/studio/">Qubry Studio</a></b> · <sub>editor · macOS · beta fechado</sub><br>
      O editor feito para agentes. Sessões, chat, mudanças, arquivos e terminal numa janela só, com o Claude Code e o Codex no centro do fluxo. Agentes conferidos antes de instalar, extensões maliciosas bloqueadas e aviso quando a pasta tem segredos.<br>
      <a href="https://qubry.dev/studio/novidades/">Novidades</a>
    </td>
    <td width="50%" valign="top">
      <img src="https://qubry.dev/assets/img/agents-icon.png?171126202806" width="48" alt="Ícone do Qubry Agents"><br>
      <b><a href="https://qubry.dev/agents/">Qubry Agents</a></b> · <sub>orquestração · macOS, Windows, Linux · beta fechado</sub><br>
      Claude Code, Codex e qualquer agente de terminal lado a lado num canvas infinito, conectados entre si.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <img src="https://qubry.dev/assets/img/terminal-icon.png?171126202806" width="48" alt="Ícone do Qubry Terminal"><br>
      <b><a href="https://qubry.dev/terminal/">Qubry Terminal</a></b> · <sub>terminal · macOS · beta fechado</sub><br>
      Todos os seus terminais num lugar só: comandos em blocos, IA que você revisa, SSH e arquivos remotos, sincronizar pastas e um servidor MCP para o Claude Code usar os seus servidores, com a sua aprovação a cada escrita.
    </td>
    <td width="50%" valign="top">
      <img src="https://qubry.dev/assets/img/countcode-icon.png?171126202806" width="48" alt="Ícone do CountCode"><br>
      <b><a href="https://qubry.dev/countcode/">CountCode</a></b> · <sub>consumo de IA · macOS · beta fechado</sub><br>
      Quanto você já usou do Claude Code e do Codex, conta por conta e pelo tipo de conta, numa barra fina abaixo da barra de menus e no rodapé do Studio, do Terminal e do Agents. Sem chave, sem nuvem.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <img src="https://qubry.dev/assets/img/db-icon.png?171126202806" width="48" alt="Ícone do Qubry DB"><br>
      <b><a href="https://qubry.dev/db/">Qubry DB</a></b> · <sub>banco de dados · Rust · macOS, Linux · beta fechado</sub><br>
      Banco de dados embutido inspirado no SQLite e reescrito do zero em Rust. Um arquivo, sem servidor.
    </td>
    <td width="50%" valign="top">
      <img src="https://qubry.dev/assets/img/qubry-mark.svg?171126202806" width="48" alt=""><br>
      <b>Beta fechado, por convite.</b><br>
      Os apps estão sendo testados com um grupo pequeno de convidados. Acompanhe as novidades em <a href="https://qubry.dev">qubry.dev</a>.
    </td>
  </tr>
</table>

## Princípios

- **Feito para agentes.** Os agentes fazem parte do fluxo de trabalho, não de uma janela de chat ao lado: sessões, mudanças e aprovações à vista.
- **Suas chaves, seus modelos.** Claude e Codex com as suas credenciais, guardadas criptografadas no Keychain do sistema.
- **Nativo e local.** Apps nativos que trabalham com os seus arquivos e o seu terminal, sem depender de uma nuvem nossa.
- **Tecnologia silenciosa.** Interfaces densas e calmas, que ficam fora do caminho até você precisar delas.
- **Seguro por padrão.** Senhas e chaves no Keychain, segredos ocultados antes de ir para a IA, extensões maliciosas bloqueadas e agentes conferidos por hash antes de instalar.
- **IA que você revisa.** Comandos, correções e mudanças sugeridos pela IA esperam a sua revisão, e você vê exatamente o que é enviado ao modelo.
- **Agentes conectados.** Os apps conversam por MCP: os agentes do Studio usam o canvas do Agents e os seus servidores pelo Terminal.
- **Sem telemetria.** Nenhum dado de uso é coletado. A IA só é chamada quando você pede, com as suas próprias chaves.

## Segurança

Os apps lidam com chaves de API, acessos a servidores e código. Cada um passou por uma revisão de segurança (novembro de 2026), com as correções já nas versões do beta:

- **Qubry Studio:** a chave da Anthropic chega só ao agente Claude; os SDKs do Claude e do Codex só instalam com o hash fixado no app; lista de extensões maliciosas do Open VSX; nenhuma extensão recebe uma conta sem pedir; aviso de `.env` e chaves na pasta da sessão; Notas cifradas.
- **Qubry Terminal:** senhas, tokens e `.env` ocultados antes de qualquer pedido à IA; histórico sem comandos com segredo; bloqueio com Touch ID que não se desliga por fora; chave ssh criada com frase; impressão digital de servidor novo em destaque; agentes só com aprovação a cada escrita.

Encontrou um problema de segurança? Fale direto com o autor em [edgo.app.br](https://edgo.app.br), sem abrir issue pública.

## Código e downloads

O código-fonte dos apps e os repositórios de downloads são privados durante o beta.

---

<sub>© 2026 Ederson Melo · by [edgo°](https://edgo.app.br)</sub>
