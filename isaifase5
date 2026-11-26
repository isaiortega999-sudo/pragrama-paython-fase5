"""
Curso: Fundamentos de Programación - 213022
Fase 5 - Evaluación Final POA
Problema 3: Reabastecimiento de inventario
Estudiante: Isai Ortega Paternina
Programa: Ingeniería de Sistemas
Código Fuente: autoría propia
"""

# Matriz de inventario:
# [Código del artículo, Nombre del artículo, Stock actual, Stock mínimo requerido]
inventario = [
    ["A001", "Teclado", 5, 10],
    ["A002", "Mouse", 20, 15],
    ["A003", "Monitor", 3, 8],
    ["A004", "Cable HDMI", 12, 12],
    ["A005", "Memoria USB", 2, 20],
    ["A006", "Impresora", 7, 5],
]


def calcular_cantidad_pedir(stock_actual, stock_minimo):
    """Devuelve la cantidad exacta a pedir de un artículo.
    Si el stock actual es menor al mínimo, pide la diferencia; si no, cero."""
    if stock_actual < stock_minimo:
        return stock_minimo - stock_actual
    return 0


def main():
    print("=== Informe de reabastecimiento ===")
    total_a_pedir = 0

    # Se recorre la matriz fila por fila
    for fila in inventario:
        nombre = fila[1]
        stock_actual = fila[2]
        stock_minimo = fila[3]

        cantidad = calcular_cantidad_pedir(stock_actual, stock_minimo)
        total_a_pedir += cantidad
        print(f"{nombre}: pedir {cantidad} unidad(es)")

    print(f"\nTotal de unidades a solicitar: {total_a_pedir}")


if __name__ == "__main__":
    main()
