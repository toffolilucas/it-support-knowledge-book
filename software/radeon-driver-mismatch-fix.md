# Correção do erro: Radeon Software and Driver Version Do Not Match ##

📌 Descrição do Problema

Ao iniciar o AMD Software (Adrenalin Edition), o sistema apresentava a mensagem: "Radeon Software and Driver Version Do Not Match." O erro indica incompatibilidade entre a versão do driver da GPU instalada no sistema e a versão do software AMD Radeon.

🖥️ Ambiente

- Sistema Operacional: Windows 10/11
- GPU: AMD Radeon - Equipamento: Notebook pessoal
- Contexto: Uso doméstico / laboratório pessoal para prática de troubleshooting

🔍 Diagnóstico

Possíveis causas identificadas: 
- Atualização automática via Windows Update
- Instalação parcial de driver
- Conflito entre versões antigas e novas
- Resíduos de instalação anterior

A GPU estava operacional no Gerenciador de Dispositivos, descartando falha física.

🛠️ Solução Aplicada

Foi realizada a remoção do driver utilizando o DDU (Display Driver Uninstaller), seguida da reinstalação do driver oficial mais recente disponibilizado pela AMD.

📋 Procedimento Técnico

1. Download das ferramentas
- DDU (Display Driver Uninstaller)
- Driver oficial no site da AMD

2. Inicialização em Modo de Segurança
- Executado `msconfig`
- Aba "Inicialização do Sistema"
- Selecionado "Modo de Segurança"
- Reinicialização do equipamento

3. Remoção completa com DDU
- Dispositivo: GPU
- Fabricante: AMD
- Opção: Clean and Restart

4. Reinstalação do driver
- Executado instalador oficial da AMD
- Instalação padrão - Reinicialização ao final do processo

✅ Resultado 

- AMD Software voltou a abrir normalmente
- Erro de incompatibilidade eliminado
- Versões de driver e software sincronizadas
- Sistema estável após reinicializações

⚠️ Observação Foi identificado método alternativo via alteração de registro:

HKEY_LOCAL_MACHINE\SOFTWARE\AMD\CN 

Porém, essa abordagem apenas altera a versão exibida e não corrige o conflito real, portanto não foi adotada. 

📚 Aprendizados 
- Importância da remoção limpa em conflitos de driver
- Impacto do Windows Update em ambientes de usuário final
- Validação da causa antes da aplicação de solução paliativa
- Documentação como parte do processo técnico

📎 Evidências - Para acompanhar o passo a passo da resolução do problema: https://youtu.be/Fef9YRBFQYU
