# telecom-analisis-2
# Predicción de Cancelación de Clientes (Churn) – TelecomX

Este proyecto implementa modelos de **Inteligencia Artificial** para predecir la cancelación de clientes en una empresa de telecomunicaciones. Se analizan los factores que influyen en el churn y se proponen estrategias de retención basadas en los resultados.

---

## 🔹 Objetivo
- Predecir qué clientes tienen mayor probabilidad de cancelar sus servicios.
- Analizar los factores que influyen en la cancelación.
- Proponer estrategias de retención para mejorar la fidelización de clientes.

---

## 🔹 Dataset
- Fuente: `TelecomX_Data.json`
- Contiene información de **clientes**, **servicios de teléfono**, **servicios de internet** y **cuentas**.
- Columnas principales:
  - `customerID`, `Churn`, `gender`, `SeniorCitizen`, `Partner`, `Dependents`
  - `tenure`, `PhoneService`, `MultipleLines`
  - `InternetService`, `OnlineSecurity`, `OnlineBackup`, `DeviceProtection`, `TechSupport`, `StreamingTV`, `StreamingMovies`
  - `Contract`, `PaperlessBilling`, `PaymentMethod`, `Charges.Monthly`, `Charges.Total`

---

## 🔹 Modelos Utilizados
Se desarrollaron dos modelos predictivos:

| Modelo                | Normalización | Accuracy |
|----------------------|---------------|---------|
| Regresión Logística   | Sí           | 79.7%   |
| Random Forest         | No           | 79.5%   |

- **Regresión Logística:** Permite interpretar coeficientes y dirección de efecto de cada variable.  
- **Random Forest:** Permite evaluar la importancia relativa de las variables y es robusto a la escala de datos.

---

## 🔹 Factores más relevantes
1. **Antigüedad del cliente (`tenure`)** – Menor antigüedad = mayor riesgo de churn.
2. **Tipo de contrato** – Contratos mes a mes aumentan cancelaciones; contratos largos reducen churn.
3. **Facturación (`Charges.Total` y `Charges.Monthly`)** – Clientes con facturación alta tienen mayor riesgo.
4. **Servicios adicionales** – Soporte técnico, seguridad online y backups reducen cancelación.
5. **Facturación electrónica** – Incentivar facturación digital mejora la experiencia y reduce fricción.

---

## 🔹 Estrategias de Retención
- Programas de bienvenida y fidelización temprana.
- Incentivos para contratos a largo plazo.
- Planes personalizados según facturación y uso.
- Promoción de servicios adicionales con soporte activo.
- Comunicación constante y beneficios para clientes nuevos.

---

## 🔹 Estructura del Proyecto
