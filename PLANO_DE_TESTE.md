# Plano de Teste Estático

| ID | Erro | Severidade | Impacto | Correção |
|----|------|------------|---------|-----------|
| 1 | SQL Injection | Alta | Comprometimento DB | PreparedStatement |
| 2 | Conexões abertas | Média | Memory Leak | Try-with-resources |
| 3 | Catches vazios | Alta | Erro silencioso | Logging apropriado |
| 4 | Credenciais expostas | Alta | Segurança | Config externa |
| 5 | Driver incorreto | Alta | Falha conexão | Corrigir nome |