# Ejemplos-bootstrap-himhervert

Espacio de trabajo para la materia de aplicaciones web interactiva.
2018/2019-1

# Bootstrap
<h5>Fecha:16/08/2018</h5>
<h3> Medidas </h3>
<ul>
    <li>Extra Small < 576px</li>
    <li>756px <= Small < 768px</li>
    <li>768px <= Medium < 992px</li>
    <li>992px <= Large < 1200px</li>
    <li>1200px <= Extra Large</li>
</ul>

<h5>Fecha:17/08/2018</h5>
#Ejercicio
<p>
1) Crear una malla que ocupe tamaño mediano y que se adapte a 2x2 en tamaño pequeño
2) Crear una malla que ocupe 2x4 en tamaño pequeño y de 4x2 en extra-pequeño
</p>

<h5>Fecha:20/08/2018</h5>
#Alineamiento
<ul>
<li>Vertical</li>

    .align-items - {start|center|end}
<li>Horizontal</li>

            .justify-content - {start|center|end|around|between}
            
</ul>

# Márgenes y Padding

{propiedad}{lados}-{tamaño}
    
    propiedad:
        m
        p
    
    lados:
        t
        b
        l
        r
        x
        y
        ninguno(aplica a todo)
    
    tamaño:
        0 - eliminar
        1 - 0.25 rem
        2 - 0.5 rem
        3 - 1 rem
        4 - 1.5 rem
        5 - 3 rem
        auto

<h5>Fecha:21/08/2018</h5>

#Tipografia
    
    Encabezados h1-h6
    Displays (1-4)

Clase .lead (texto estilizado)

*Texto*
    
    .text - {sm|md|lg} - {justify|left|center|right}

* .lowercase
* .uppercase
* .capitalize

*Imágenes*
    
* .img-fluid
* .img-thumbnail

*Bordes*

    .border - {top|bottom|left|right} - {0}

* _colores_
        
        .border - {primary|secondary|success|danger|info|warning}

*Redondeado(Borde)*
    
    .rounded - {top|right|bottom|left|circle}

*Propiedad Display (CSS)*

    1. inline
    2. block
    3. inline-block

    .d-none
    .d-inline
    .d-block
    .d.inline-block

    .d - {sm|md|lg} - {none|inline|block|inline-block} 
