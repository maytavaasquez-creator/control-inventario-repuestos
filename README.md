# Control de inventario de repuestos

Proyecto académico para aplicar **Git y GitHub** a un problema real de una organización: el control de inventarios de una empresa de repuestos.

## Problemática

- Productos con **stock en cero** que generan ventas perdidas.
- **Mercadería innecesaria** (excedentes sobre el stock máximo) que inmoviliza capital.
- El control se lleva en archivos Excel que se modifican sin historial: no se sabe quién cambió qué ni cuándo, y las versiones se duplican (`inventario_final`, `inventario_final2`...).

## Qué resuelve Git y GitHub

- Historial completo de cambios del archivo de inventario.
- Ramas para probar mejoras sin afectar la versión estable.
- Trabajo colaborativo ordenado mediante Pull Requests.
- Posibilidad de volver a una versión anterior.

## Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `inventario.xlsx` | Libro de inventario (datos de ejemplo, ficticios) |
| `README.md` | Este documento |
| `.gitignore` | Excluye archivos temporales de Excel |

## Estructura de ramas

- `main`: versión estable.
- `develop`: integración de mejoras.
- `feature/alerta-stock-minimo`: agrega la columna Estado (SIN STOCK / REPONER / OK).
- `feature/reporte-excedentes`: agrega el cálculo de excedentes y una hoja Resumen.

## Versiones

| Versión | Cambio |
|---|---|
| v0.1.0 | Inventario base |
| v1.0.0 | Alertas de stock y reporte de excedentes integrados |
