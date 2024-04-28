# JSON
import json

d1 = {
  'Pessoa 1': {
    'nome': 'João',
    'idade': 25,
    'cidade': 'São Paulo',
  },
  'Pessoa 2': {
    'nome': 'Maria',
    'idade': 30,
    'cidade': 'Rio de Janeiro',
  },
}

d1_json = json.dumps(d1, indent=True)

with open('abc.json', 'w+', encoding="utf-8") as file:
  file.write(d1_json)
