# aula2
Exercicio1

db.Alunos.insert({ "name":"Leonardo Quintao", "birthday":ISODate("1986-11-27"), "cursadas":"ILE", "cursando":"NSQ" })
db.Alunos.insert({ "name":"Eduardo Cardoso", "birthday":ISODate("1987-04-22"), "cursadas":"ILE", "cursando":"NSQ" })
db.Alunos.insert({ "name":"Briner Homem", "birthday":ISODate("1988-11-07"), "cursadas":"ILE", "cursando":"NSQ" })
db.Alunos.insert({ "name":"Fabricio", "birthday":ISODate("1987-12-09"), "cursadas":"ILE", "cursando":"NSQ" })
db.Alunos.find({},{date:1, _id:0}).sort({date:1})
db.Alunos.update({ "name":"Leonardo Quintao"}, {$set:{"notaNSQ":5}})
db.Alunos.remove({
... "name":"Briner Homem",
... })
)
