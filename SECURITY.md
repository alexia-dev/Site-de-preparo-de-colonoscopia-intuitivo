# Segurança

## Não inserir dados de pacientes
Esta versão é um protótipo estático. Não coleta nem deve armazenar nome, CPF, telefone, prontuário, diagnóstico, foto, documento ou qualquer dado identificável de paciente.

## Painel
O painel atual é apenas uma demonstração local e não tem autenticação real. Não o utilize para administrar conteúdo em produção. Para uso real:
- autenticação robusta (Firebase Auth ou backend Spring Boot);
- autorização por função (somente equipe autorizada);
- regras server-side, nunca confiar em esconder botões no frontend;
- trilha de auditoria de alterações e aprovação clínica;
- MFA para contas administrativas, quando possível;
- backups e política de retenção;
- proteção de segredos em variáveis de ambiente;
- revisão de segurança e LGPD.

## Conteúdo clínico
Toda orientação deve ser aprovada pelo responsável clínico. Não incluir doses, suspensões ou ajustes de medicamentos sem protocolo oficial validado. Em caso de dúvida, o paciente deve contatar a clínica/equipe médica.
