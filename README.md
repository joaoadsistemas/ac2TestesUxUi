# Sistema de Login - Análise de Código

## Erros Encontrados
1. Segurança
   - SQL Injection na construção da query
   - Credenciais expostas no código
   - Senha sem criptografia

2. Gestão de Recursos
   - Conexões não fechadas
   - Statement não fechado
   - ResultSet não fechado

3. Tratamento de Exceções
   - Blocos catch vazios
   - Exceções genéricas
   - Sem logging

4. Design e Implementação
   - Driver MySQL incorreto
   - Variáveis públicas
   - Sem validação de entrada