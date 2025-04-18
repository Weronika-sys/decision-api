# Decision API

Adres:  http://localhost:5000/api/v1.0/predict?x1=3.2&x2=4.0

Prosty serwis API napisany w Pythonie Flask, który zwraca predykcję na podstawie dwóch liczb.

## Zasada działania modelu

- Jeśli `x1 + x2 > 5.8`, API zwraca `prediction: 1`
- W przeciwnym razie zwraca `prediction: 0`
- Jeśli liczba nie zostanie podana, przyjmowana jest wartość 0

### Przykład:

- `x1=2.5&x2=1.0` → wynik będzie `prediction: 0`  
- `x1=5.0&x2=1.0` → wynik będzie `prediction: 1`  
- `x2=4.2` (bez `x1`) → `x1` zostanie przyjęte jako `0`