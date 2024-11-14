graph TD
    1[Início] --> 2[conectarBD]
    2 --> 3{try conexão}
    3 -->|sucesso| 4[criar conexão]
    3 -->|falha| 5[catch]
    4 --> 6[return conn]
    5 --> 6
    6 --> 7[verificarUsuario]
    7 --> 8[montar SQL]
    8 --> 9{try query}
    9 -->|sucesso| 10{rs.next}
    10 -->|true| 11[set result]
    10 -->|false| 12[return result]
    11 --> 12
    9 -->|falha| 13[catch]
    13 --> 12