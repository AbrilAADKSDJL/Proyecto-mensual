// en la carpeta models en bunieslogic

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;


namespace BusinessLogic.Models
{
    public class ArticuloDto
    {
        public int IdProducto { get; set; }
        public int? IdCategoria { get; set; } 
        public string Codigo { get; set; }
        public string CodigoBarra { get; set; }
        public string Categoria { get; set; } 
        public string Nombre { get; set; }
        public string Descripcion { get; set; }
        public string Marca { get; set; }
        public DateTime? Vencimiento { get; set; }
        public string? Lote { get; set; }
        public int? AvisoVencimientoDias { get; set; }
        public decimal PrecioCompra { get; set; }
        public decimal PrecioVenta { get; set; }
        public int StockActual { get; set; }
        public int StockMinimo { get; set; }
        public int StockIdeal { get; set; }
        public int StockMaximo { get; set; }
        public string TipoStock { get; set; }

        public ArticuloDto()
        {
            Codigo = string.Empty;
            CodigoBarra = string.Empty;
            Categoria = string.Empty;
            Nombre = string.Empty;
            Descripcion = string.Empty;
            Marca = string.Empty;
            TipoStock = string.Empty;
        }
    }
}