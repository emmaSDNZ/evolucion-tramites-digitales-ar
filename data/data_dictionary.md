# 7️⃣ Diccionario de datos (data_dictionary.md)

| Columna                        | Descripción                                                   |
|--------------------------------|---------------------------------------------------------------|
| id_tramite                     | Identificador único del trámite                               |
| nombre_tramite                 | Nombre oficial del trámite                                    |
| organo_rector                  | Organismo responsable                                         |
| fecha_publicacion_produccion   | Fecha de publicación en la plataforma                         |
| marca_arancelado               | Indica si el trámite es arancelado (original)                 |
| arancelado                     | Columna booleana derivada de `marca_arancelado`               |
| link_de_acceso                 | Enlace directo al trámite                                     |
| validador_identidad            | Lista de validadores de identidad utilizados                  |
| valida_AFIP                    | Columna booleana si AFIP es validador                         |
| valida_Mi_argentina            | Columna booleana si Mi Argentina es validador                 |
| valida_ANSES                   | Columna booleana si ANSES es validador                        |
| valida_DNI                     | Columna booleana si DNI es validador                          |
| valida_NIC-AFIP                | Columna booleana si NIC-AFIP es validador                     |
| anio                           | Año de publicación                                            |
| mes                            | Mes de publicación                                            |
| trimestre                      | Trimestre de publicación                                      |
| dia                            | Día del mes de publicación                                    |
| dia_semana                     | Nombre del día de la semana                                   |

---
