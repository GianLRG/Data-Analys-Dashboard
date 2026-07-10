# 📊 Análisis de Ventas y Devoluciones – GYM Barracuda

Dashboard interactivo en Excel para analizar el desempeño de ventas de una empresa de ropa deportiva en línea, con el objetivo de identificar la causa raíz del aumento de devoluciones a lo largo del año y su impacto financiero.

![Dashboard](https://github.com/GianLRG/Data-Analys-Dashboard/blob/main/Dashboard.jpg)

## 📌 Contexto

GYM Barracuda vende a través de dos canales:
- **Venta propia**: publicidad pagada directamente por la empresa (Website, Instagram, Facebook, Youtube).
- **Influencers/Afiliados**: creadores de contenido que promocionan productos a cambio de una comisión por venta.

A lo largo del año, la empresa reportó un aumento notable en devoluciones, lo cual genera pérdidas (la mercancía devuelta se vende posteriormente en Outlet con 35% de descuento). Se me encargó construir un dashboard para diagnosticar la causa y cuantificar el impacto en las ganancias.

## 🎯 Objetivo

Construir un dashboard 100% interactivo (con segmentadores) que responda:
1. ¿Cuál es el desempeño general de ventas, devoluciones y comisiones?
2. ¿Qué influencers generan más ventas y más devoluciones?
3. **¿Por qué están subiendo las devoluciones y qué se puede hacer al respecto?**

## 🛠️ Metodología

- Limpieza y modelado de una base de datos de ~63,000 transacciones (ventas y devoluciones mezcladas en una sola columna, requiriendo filtrado por `Tipo de Orden`).
- Tablas dinámicas para calcular KPIs y la tabla de Top 10 Influencers.
- Gráficas dinámicas (ventas por mes, ventas por medio de adquisición).
- Segmentadores por Sexo y Categoría conectados a todas las visualizaciones.
- Análisis comparativo de tasa de devolución por canal (Propio vs. Influencer) para aislar la causa específica.

## 📈 KPIs incluidos

| KPI | Descripción |
|---|---|
| Ventas Totales | Ventas brutas en dólares (excluye devoluciones) |
| Devoluciones | Valor devuelto en $ y como % de ventas brutas |
| Ventas Propias / de Influencers | Desglose por canal |
| Comisiones a Influencers | Total pagado, incluyendo comisión sobre ventas devueltas |
| Ventas Netas | Ventas − devoluciones − comisiones |
| Pérdidas totales | Descuento de Outlet (35%) + comisiones pagadas sobre mercancía devuelta |
| Top 10 Influencers | Ventas brutas, devolución, venta neta y % de devolución por influencer |

## 🔎 Hallazgo principal

La tasa de devolución del canal **Propio** se mantuvo estable todo el año (2.5%–6.8%), mientras que la del canal **Influencer** subió de forma sostenida (7% → hasta 20% mensual). La causa: los influencers **conservan su comisión aunque el producto sea devuelto**, por lo que no tienen incentivo económico para promocionar con precisión (tallas, expectativas del producto, etc.).

**Recomendación:** condicionar el pago de comisión a que la venta no se devuelva dentro de un plazo determinado.

## 📁 Estructura del repositorio

```
├── Ventas_en_Linea.xlsx     # Archivo con las hojas: Datos, Análisis, Dashboard
├── assets/                  # Capturas de pantalla del dashboard
└── README.md
```

## 🧰 Herramientas utilizadas

- Microsoft Excel (Tablas dinámicas, Gráficas dinámicas, Segmentadores, Fórmulas)

## Autor

Proyecto de práctica de análisis de datos (Nivel Yellow Belt).
