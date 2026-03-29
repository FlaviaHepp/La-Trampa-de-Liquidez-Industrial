# 📉La Trampa de Liquidez Industrial

Detección de Riesgo de Ejecución por Falta de Contrapartida

## 🧠Descripción del Proyecto

Este proyecto identifica industrias en una situación peligrosa de liquidez, donde el interés del mercado se está evaporando (volumen en caída) al mismo tiempo que la tendencia de precios se fortalece (ADX alto).

Este escenario es conocido como una trampa de liquidez:
- el precio se mueve con fuerza, pero cada vez hay menos participantes, lo que puede provocar movimientos violentos, gaps inesperados y slippage severo.

## 🎯Insight Clave

- ¿Qué industrias muestran una tendencia fuerte (ADX > 30) mientras el volumen negociado cae de forma significativa en los últimos días?

Este patrón suele preceder:
- Flash moves
- Dificultad para ejecutar órdenes grandes
- Riesgo oculto para fondos e inversores institucionales

## 💼Valor de Negocio

⚠️ Alerta temprana de riesgo de ejecución
Ideal para desks institucionales, hedge funds y gestores de riesgo.

📊 Optimización del sizing de posiciones
Evita entrar “grande” en mercados donde no hay contrapartida real.

🌪️ Prevención de slippage extremo
Especialmente relevante en commodities, small caps o industrias cíclicas.

## 🧮Metodología

El modelo combina tres elementos clave:
- Fuerza de la tendencia
- Se utiliza el ADX (14) como proxy de direccionalidad fuerte.
- Umbral: ADX > 30.
- Dinámica del volumen
- Se compara el volumen promedio reciente contra períodos previos.
- Se detecta una caída estructural del volumen.
- Análisis a nivel industrial
- El agrupamiento por industria permite detectar riesgos sistémicos, no solo problemas aislados de un ticker.

## 🗂️Tablas Utilizadas

- precios_diarios
- Datos de precio y volumen.
- indicadores_tecnicos
- Incluye ADX y otros indicadores de tendencia.
- tickers
- Metadatos de industria y clasificación.

## 📈Interpretación de Resultados

Las industrias que aparecen en el resultado cumplen simultáneamente:
- ✔️ Tendencia fuerte y definida
- ❌ Volumen decreciente (desinterés del mercado)
- 👉 Conclusión: el movimiento actual puede continuar, pero con un riesgo elevado de ejecución y volatilidad explosiva.

## ⚠️Advertencia

Este insight no es una señal direccional de compra o venta por sí sola.
Es una señal de riesgo estructural, que debe combinarse con:
- gestión de tamaño
- análisis de volatilidad
- contexto macro o fundamental

## 🚀Casos de Uso Típicos

- Control de riesgo en portfolios sectoriales
- Ajuste de liquidez antes de eventos macro
- Detección de mercados frágiles antes de un breakout

## 👤Autora
Flavia Hepp Proyecto de SQL aplicó un análisis de riesgo basado en eventos.

***
⚠️📉 **Cuando la liquidez desaparece… pero la tendencia se fortalece**

Hay señales que no aparecen en el precio…
pero pueden ser incluso más peligrosas.

👉 Analicé un patrón que llamo **“trampa de liquidez”** a nivel industrial:

* 📉 Volumen en caída (menos participación)
* 📈 ADX alto (>30) → tendencia fuerte

💡 **Insight clave:**
Cuando una tendencia se fortalece mientras la liquidez cae, el mercado se vuelve **frágil**.
Y eso puede desencadenar movimientos violentos por falta de contrapartida.

---

📊 **¿Qué medí?**

* Fuerza de tendencia (ADX promedio por industria)
* Cambio en volumen reciente vs. histórico
* Identificación de industrias con:

  * Tendencias fuertes
  * Volumen decreciente

---

🧠 **¿Cómo interpretarlo?**

* Alta tendencia + baja liquidez → mercado “vacío”
* Menos participantes → mayor impacto por orden
* Mayor probabilidad de:

  * Slippage
  * Movimientos bruscos
  * Rupturas desordenadas

---

⚡ **¿Por qué importa?**

Porque afecta directamente la ejecución:

* Estrategias pueden parecer rentables… pero no ejecutables
* Riesgo oculto en posiciones grandes
* Importante para fondos e institucionales

---

📌 Pregunta para la comunidad:
¿Alguna vez una estrategia falló no por la señal… sino por la falta de liquidez?

#QuantFinance #Trading #DataScience #MarketMicrostructure #Liquidity #RiskManagement #Alpha #Analytics
