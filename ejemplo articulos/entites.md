
using System;
using System.Collections.Generic;

namespace DataAccess.Entities
{
    public class Articulo
    {
        public int IdProducto { get; set; }
        public string Codigo { get; set; } = string.Empty;
        public string? CodigoBarra { get; set; }

        // FK a Categoria
        public int IdCategoria { get; set; }
        public Categoria? Categoria { get; set; }

        public string Nombre { get; set; } = string.Empty;
        public string? Descripcion { get; set; }
        public string? Marca { get; set; }
        public DateTime? Vencimiento { get; set; }
        public string? Lote { get; set; }
        public int? AvisoVencimientoDias { get; set; }

        public decimal PrecioCompra { get; set; }
        public decimal PrecioVenta { get; set; }

        public int StockActual { get; set; }
        public int StockMinimo { get; set; }
        public int StockIdeal { get; set; }
        public int StockMaximo { get; set; }
        public string TipoStock { get; set; } = string.Empty;

        // Navegación inversa
        public ICollection<DetalleCompra>? DetallesCompra { get; set; }
        public ICollection<MovimientoInventario>? Movimientos { get; set; }
        public ICollection<Scrap>? Scraps { get; set; }
    }
}
