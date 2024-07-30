# PT-Juan-Navarro

Subí una copia de mi script de sql server debido a que mi base de datos era local

modificar en el appsettings.jason el servidor donde almacena su base de datos
"ConnectionStrings": {
  "Cadena_con": "Server=DESKTOP-H9BAB7Q\\SQLEXPRESS;Database=Seguros;Trusted_Connection=True;TrustServerCertificate=True;"
}

Lo mismo con el archivo SegurosContext.cs en la siguiente seccion:
    protected override void OnConfiguring(DbContextOptionsBuilder optionsBuilder)
#warning To protect potentially sensitive information in your connection string, you should move it out of source code. You can avoid scaffolding the connection string by using the Name= syntax to read it from configuration - see https://go.microsoft.com/fwlink/?linkid=2131148. For more guidance on storing connection strings, see https://go.microsoft.com/fwlink/?LinkId=723263.
        => optionsBuilder.UseSqlServer("Server=DESKTOP-H9BAB7Q\\SQLEXPRESS;Database=Seguros;Trusted_Connection=True;TrustServerCertificate=True;");
