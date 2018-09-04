# Ejemplos-bootstrap-himhervert

Espacio de trabajo para la materia de aplicaciones web interactiva.
2018/2019-1

# Bootstrap
#####Fecha:16/08/2018

<h3> Medidas </h3>
<ul>
    <li>Extra Small < 576px</li>
    <li>756px <= Small < 768px</li>
    <li>768px <= Medium < 992px</li>
    <li>992px <= Large < 1200px</li>
    <li>1200px <= Extra Large</li>
</ul>
 
#####Fecha:17/08/2018
#Ejercicio
<p>
1) Crear una malla que ocupe tamaño mediano y que se adapte a 2x2 en tamaño pequeño
2) Crear una malla que ocupe 2x4 en tamaño pequeño y de 4x2 en extra-pequeño
</p>

#####Fecha:20/08/2018
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

#####Fecha:21/08/2018

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

# Componentes

#####Fecha:23/08/2018

* Formularios
* Tablas
* Modales
* Alertas
* Carruseles

*Formularios*

Cada Elemento requiere un clase del tipo .form-control para darle un estilo en bootstrap
    
    <div class="form-control"></div>

Una clase .form-group para agrupar elementos juntos en un mismo grupo.

    <div class="form-group"></div>


#Validación de Formularios

#####Fecha:27/08/2018

La validaicon puede ser de 2 formas

a) Default(navegador/HTML5)
    
    required...

b) Personalizado(Bootstrap, JavaScript, jQuery)

*Bootstrap*

    * .form.needs-validation
    * .valid-feedback
    * .invalid-feedback

Al obtener estos eventos se deben de recuperar con JavaScript

    addEventListener('submit',function(evento){
        if(formulario.checkValidity()===false)
            evento.preventDefault();
    }
    formulario.classList.add('was-validated');


# Alertas y Modales

#####Fecha:28/08/2018

*ALERT*

Cuenta por default las clases

    button.close
    .data-dismiss="alert"

todo debe estar encerrado en un div
y puede llevar colores de bootstrap

    .alert
    .alert-warning
    .alert-heading

*MODAL*

Contiene un Encabezado, contenido y pie de pagina.
Cuenta con las clases:

    button.close
    .data-dismiss="modal"

    .modal-header
    .modal-body
    .modal-footer

    .modal id="mi-modal"

Requiere un boton para abrir el modal

    button.data-toggle="modal"
    data-target="#mi-modal"

Cuenta con los botones de cancelar y aceptar para decidir que acción reallizar con el modal

    .close
    .data-dismiss="modal"

La "X" para cerrar el modal o alert puede ser con la el tipo:

    times
    

#Navbar

#####Fecha:30/08/2018

||Logo|Inicio|Servicios|Contacto||

*Contenedor* 

    div.navbar

*Logo*
    
    a.navbar-brand
*Menu* (InicioServicios|Contacto)

    ul.navbar-nav

*Items*

    li.nav-item

*Link*

    a.nav-link
    
*Colores*

    .navbar-light
    .navbar-dark

*Responsibidad*

    .navbar-expand-md

*Boton de Hamburguesa*
<hr>
Toggler = Intercambio de estado.

    span.navbar-toggler-icon
    button.navbar-toggler
    data-toggle="collapse"
    data-target="

Todos los elementos que vayan dentro del boton deben de estar en un div con un id
    
    id ="miMenu"
    div.collapse
    .navbar-collapse
    #miMenu


## Carrusel

##### Fecha:31/08/2018

<p>Sección para llamar la atención del usuario, generalmente se maneja por imagenes y se muestran una a la vez.</p>
<p>Tambien cuenta con controles que permiten cambiar de imagen.</p>

*Contenedor*

    div.carousel
    .slide

    data-ride="carousel"
    data-interval="1000"
    id="#Mi-Carousel"

*Contenido de muestra*

    div.carousel-inner

**Cada imagen se maneja como:**

    div.carousel-item
    
    * El primer item debe de llevar la clase: *
    .active
**Texto para cada imagen**

    div.caroulser-caption

**Boton anterior/siguiente**

    a.carousel-control-next
    a.carousel-control-pre

**Boton de seleccionar indice**

    ol/ul.carousel-indicators
        
        li.active
            data-target="#Mi-Carousel"
            data-slide-to="0"

## Tarjetas (Cards)

##### Fecha:03/09/2018

Contiene un encabezado, un contenido y un pie de página.

La unica desventaja es que no es responsivo, pero se pueden trabajar varias tarjetas en una sola ventana.

    div.card
        >
            div.card-header
            img.card-img-{top|bottom}
            El body puede llevar dentro una imagen
            div.card-body
            div.card-footer

El uso mas comun para este elemento, es para mostrar algun producto. Tienen la ventaja es brindar una estructura para acomodar tarjetas con diferentes contenidos.

Cuando se usa el elemento
> div.card-group

Acomoda diversas tarjetas con el misma altura.

El elemento:
>div.card-desk

Permite que los elementos esten acomodados de diversos tamaños.

El elemento:

    div.card-columns

Permite que los elementos sean acomodados de arriba hacia abajo, continuando de izquierda a derecha.


## Acordeón (Collapse)
##### Fecha:04/09/2018

El acordeón permite ocultar elementos cuando se desee.

    div.card
        a data-toggle="collapse"
        href="#id"
        div.card-header
        div.collapse
        div.card-body
    /div

