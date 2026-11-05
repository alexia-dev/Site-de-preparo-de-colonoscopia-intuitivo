# Endoimagem | Preparo de Colonoscopia

Site responsivo para orientar pacientes da Endoimagem sobre o preparo de colonoscopia e oferecer um painel administrativo simples para editar o conteúdo aprovado pela equipe.

> **Importante:** este repositório é uma base técnica. O conteúdo clínico deve ser revisado e aprovado pelo Dr. Nicácio Serrano / responsável clínico antes da publicação. Não use este site para prescrever medicamentos ou alterar orientações médicas.

## O que está incluído
- Página pública responsiva para pacientes.
- Seleção da data e horário do exame, com linha do tempo ilustrativa.
- Checklist local no dispositivo (não envia dados à clínica).
- Botão para compartilhar o link via WhatsApp.
- Painel administrativo demonstrativo para editar textos e contatos.
- GitHub Pages para publicação gratuita.
- Avisos de privacidade e checklist de implantação.

## Estado atual e segurança
Esta primeira versão é **frontend estático**. O painel usa armazenamento local do navegador e **não é autenticação segura**. Não coloque dados de pacientes, senhas, informações clínicas identificáveis nem publique o painel como ferramenta administrativa real até conectar autenticação e banco de dados seguros (ex.: Firebase Auth + Firestore com regras restritivas ou backend próprio). O botão de administração é uma demonstração para validar UX.

## Publicação gratuita com GitHub Pages
1. Abra **Settings → Pages** no repositório.
2. Em **Build and deployment**, selecione **GitHub Actions**.
3. Faça push na branch `main`; o workflow `.github/workflows/pages.yml` publica o site.
4. A URL aparecerá na seção Pages após o primeiro deploy.

## Personalização
Edite `index.html`:
- Nome e identidade visual.
- Contatos e endereço.
- Conteúdo de preparo — somente após validação clínica.
- Links de WhatsApp.

## Antes de usar com pacientes
- [ ] Aprovação clínica documentada de cada instrução, horário e alerta.
- [ ] Confirmar telefone, endereço e contatos oficiais.
- [ ] Configurar autenticação real para administração.
- [ ] Remover/evitar armazenamento local de qualquer dado pessoal.
- [ ] Validar acessibilidade, celular, impressão e links.
- [ ] Revisar política de privacidade e LGPD com responsável da clínica.
- [ ] Testar com equipe e pacientes voluntários antes de divulgar.

## Stack
HTML, CSS e JavaScript sem build, para facilitar manutenção e publicação estática.
