- 👋 Hi, I’m @Dfacundodperera
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---import ccxt
import pandas as pd

# Inicializar el intercambio (exchange)
exchange = ccxt.binance()  # Puedes cambiar a cualquier otro exchange compatible

# Obtener todos los pares de trading disponibles
markets = exchange.load_markets()

# Crear un diccionario para almacenar los datos de los precios
prices_data = {}

# Obtener los precios de cierre para cada par de trading durante los últimos 6 días (para calcular 5 días de cambio)
for symbol in markets:
    try:
        # Obtener datos históricos de precios
        ohlcv = exchange.fetch_ohlcv(symbol, timeframe='1d', limit=6)
        # Extraer solo los precios de cierre
        closes = [ohlcv[i][4] for i in range(len(ohlcv))]
        # Almacenar los precios de cierre en el diccionario
        prices_data[symbol] = closes
    except Exception as e:
        print(f"Error obteniendo datos para {symbol}: {e}")

# Crear un DataFrame de pandas con los datos de los precios
df = pd.DataFrame(prices_data)

# Calcular la variación de precio para cada par de trading
df['change'] = df.pct_change(axis=1).fillna(0)

# Filtrar los pares de trading que han subido durante los últimos 5 días consecutivos
filtered_pairs = df[df['change'].apply(lambda x: (x > 0).rolling(window=5).sum().iloc[-1] == 5)].index.tolist()

print("Criptomonedas que han subido durante los últimos 5 días consecutivos:")
print(filtered_pairs)     
Dfacundodperera/Dfacundodperera is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
