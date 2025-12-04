using DataAccess.Entities;
using System.Collections.Generic;

namespace DataAccess.Repositories
{
    public interface IArticuloRepository
    {
        Articulo? GetById(int id);
        IEnumerable<Articulo> GetAll();
        void Add(Articulo articulo);
        void Update(Articulo articulo);
        void Delete(int id);
        bool ExistsByCodigo(string codigo, int? excludeId = null);
        bool ExistsByCodigoBarra(string codigoBarra, int? excludeId = null);
    }
}