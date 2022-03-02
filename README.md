clase RNA-seq LCGEJ2022
================

Presentación:
<https://mpadilla905.github.io/clase_RNA-seq_LCGEJ2022/slides_RNA-seq.html#1>

Contenido inspirado en curso de RNA-seq de la Red Mexicana de
Bioinformática: <https://comunidadbioinfo.github.io/minicurso_abr_2021/>

### Clonar este repositorio

``` bash
git clone https://github.com/mpadilla905/clase_RNA-seq_LCGEJ2022.git
```

Recuerda hacer tu git token primero. Ve a
<https://github.com/settings/profile> &gt; Selecciona
`<> Developer Settings` de la lista &gt; `Personal Access Tokens` &gt;
`Generate new token`

-   Dale un nombre
-   Selecciona la duración del token
-   Selecciona los permisos que tendrás con dicho token en github

Ve a `Generate token` &gt; **Guarda muy bien** en algún archivo este
token pues no se te volverá a mostrar en github de nuevo.

------------------------------------------------------------------------

### Requisitos

**Programas**

-   [salmon](https://combine-lab.github.io/salmon/getting_started/)
-   R &gt; 4.0
-   RStudio
-   Paquetes de R con Bioconductor
    -   Biconductor
    -   DESeq2
    -   tximport

``` r
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")
BiocManager::install(version = "3.13")

paquetes = c("DESeq2", "tximport")
BiocManager::install(paquetes)
```

-   Paquetes de R
    -   wordcloud
    -   RColorBrewer
    -   tidyverse

``` r
install.packages("tidyverse")
installed.packages("wordcloud")
install.packages("RColorBrewer")
```

  

------------------------------------------------------------------------

  

### Agenda

| Día | Temas                   | Link a presentación                                                           |
|-----|-------------------------|-------------------------------------------------------------------------------|
| 1   | Overview y Pre Análisis | <https://mpadilla905.github.io/clase_RNA-seq_LCGEJ2022/slides_RNA-seq.html#2> |
