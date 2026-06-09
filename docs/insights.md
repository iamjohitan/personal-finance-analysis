# 💡 Key Insights — Personal Finance Analysis

Análisis basado en **13,115 transacciones** de 150 usuarios entre **2021 y 2024**.

---

## 📊 Resumen ejecutivo

| KPI | Valor |
|---|---|
| Total ingresos | $130,565,726 |
| Total gastos | $152,651,019 |
| Ahorro neto | -$22,085,293 |
| Tasa de ahorro global | **-16.92%** |

El dataset refleja una situación de déficit financiero sostenido: los gastos superaron los ingresos en un 16.92% durante el período completo. Sin embargo, el análisis año a año revela una tendencia más matizada.

---

## 📅 Tendencia anual

| Año | Ingresos | Gastos | Ahorro neto |
|---|---|---|---|
| 2021 | $25,526,806 | $41,854,666 | **-$16,327,860** |
| 2022 | $32,287,847 | $37,716,614 | **-$5,428,767** |
| 2023 | $33,367,715 | $29,895,795 | **+$3,471,920** ✅ |
| 2024 | $39,383,358 | $43,183,944 | **-$3,800,586** |

**Hallazgo clave:** La salud financiera mejoró progresivamente de 2021 a 2023, alcanzando el único año con ahorro positivo en 2023. Sin embargo, 2024 volvió a registrar déficit a pesar de tener los ingresos más altos del período — señal de que los gastos crecieron más rápido que los ingresos.

---

## 📂 Distribución del gasto por categoría

| Categoría | Transacciones | Total gastado | % del total |
|---|---|---|---|
| Rent | 2,153 | $44,951,173 | 29.45% |
| Food | 2,724 | $35,124,685 | 23.01% |
| Entertainment | 1,075 | $15,506,940 | 10.16% |
| Utilities | 1,269 | $15,318,951 | 10.04% |
| Travel | 1,597 | $13,147,617 | 8.61% |
| Education | 843 | $12,427,519 | 8.14% |
| Health | 504 | $5,486,322 | 3.59% |
| Others | 202 | $4,990,001 | 3.27% |

**Hallazgos:**
- **Rent y Food concentran el 52.46%** de todos los gastos — más de la mitad del presupuesto va a necesidades básicas.
- **Entertainment y Utilities** están casi empatados en ~10% cada uno, siendo los siguientes gastos más relevantes.
- **Health representa solo el 3.59%** del gasto total, lo que puede indicar subutilización de servicios de salud o buena condición general de los usuarios.
- **Education (8.14%)** es un gasto relevante, sugiriendo inversión activa en formación.

---

## 💳 Métodos de pago

| Método | Transacciones | % de uso |
|---|---|---|
| Card | 3,101 | 24.14% |
| Cash | 3,066 | 23.87% |
| Bank Transfer | 3,060 | 23.82% |
| UPI | 2,987 | 23.25% |

**Hallazgo:** La distribución entre los 4 métodos de pago es prácticamente equitativa (~24% cada uno), lo que indica que los usuarios no tienen una preferencia marcada por un método en particular. Esto también refleja la diversidad del dataset al incluir usuarios con distintos perfiles financieros.

---

## 🔍 Conclusiones generales

1. **El déficit financiero es estructural en 3 de 4 años**, con 2023 como única excepción positiva.
2. **Los gastos fijos (Rent + Food) dominan el presupuesto** — cualquier estrategia de ahorro debe enfocarse en reducir estos dos primeros.
3. **Los ingresos crecen año a año** ($25M en 2021 → $39M en 2024), pero los gastos crecen a un ritmo similar o mayor, impidiendo la acumulación de ahorro sostenido.
4. **2024 es el año de mayor ingreso pero también de mayor déficit reciente**, lo que sugiere un aumento en gastos discrecionales (Entertainment, Travel) paralelo al aumento de ingresos.
5. **Los métodos de pago digitales (Card + UPI + Bank Transfer) representan el 71.12%** de las transacciones, indicando una población financieramente digitalizada.

---

## 🛠️ Nota metodológica

- Se filtraron transacciones con `amount < 1` y `amount > 999,999` por ser outliers del dataset sucio original.
- Las categorías fueron normalizadas desde 47 variantes textuales a 10 categorías limpias usando Python/pandas.
- Los métodos de pago fueron estandarizados directamente en MySQL con un UPDATE posterior a la carga.
- Dataset original: [BudgetWise Personal Finance Dataset — Kaggle](https://www.kaggle.com/datasets/mohammedarfathr/budgetwise-personal-finance-dataset)
