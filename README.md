# Chuleta de Vuetify 3

## Breakpoints

Vuetify 3 utiliza breakpoints para adaptar la apariencia de tu aplicación a diferentes tamaños de pantalla. Puedes utilizar clases de breakpoint en tus elementos para controlar su visibilidad en función del tamaño de la pantalla.

- `xs`: Extra pequeño
- `sm`: Pequeño
- `md`: Mediano
- `lg`: Grande
- `xl`: Extra grande

Ejemplo de uso de clase de breakpoint:

```html
<v-btn class="d-sm-none">Visible en pantallas pequeñas y superiores</v-btn>
```

## Flex Direction

La propiedad de dirección flex (`flex-direction`) te permite controlar la dirección en la que se apilan los elementos flex dentro de un contenedor. Vuetify 3 proporciona clases útiles para controlar esta propiedad.

- `.flex-{value}`: Controla la dirección flex en todos los tamaños de pantalla.
- `.flex-{breakpoint}-{value}`: Controla la dirección flex en un breakpoint específico.

Valores de dirección flex disponibles:

- `row`: Los elementos flex se apilan horizontalmente en la misma dirección del flujo del contenido.
- `row-reverse`: Los elementos flex se apilan horizontalmente en la dirección opuesta al flujo del contenido.
- `column`: Los elementos flex se apilan verticalmente, uno encima del otro.
- `column-reverse`: Los elementos flex se apilan verticalmente en orden inverso.

Ejemplo de uso de clases de dirección flex:

```html
<div class="flex-row">Elementos flex en dirección horizontal.</div>
<div class="flex-column-reverse">Elementos flex en dirección vertical inversa.</div>
```
## Flex Justify

Las clases de "justify" en Vuetify 3 te permiten controlar cómo se distribuyen los elementos dentro de un contenedor flex a lo largo del eje principal. Estas clases afectan la alineación horizontal de los elementos.

- `.justify-{value}`: Controla la justificación en todos los tamaños de pantalla.
- `.justify-{breakpoint}-{value}`: Controla la justificación en un breakpoint específico.

Valores de justificación disponibles:

- `start`: Alinea los elementos al principio del contenedor.
- `end`: Alinea los elementos al final del contenedor.
- `center`: Alinea los elementos en el centro del contenedor.
- `space-between`: Distribuye uniformemente los elementos a lo largo del eje principal, con el primer elemento al principio y el último al final.
- `space-around`: Distribuye uniformemente los elementos a lo largo del eje principal, con espacio adicional alrededor de cada elemento.

Ejemplo de uso de clases de justificación flex en Vuetify:

```vue
<template>
  <v-container>
    <v-row class="justify-start">
      <v-col>Elemento al principio</v-col>
      <v-col>Elemento al principio</v-col>
    </v-row>
    
    <v-row class="justify-center">
      <v-col>Elemento en el centro</v-col>
      <v-col>Elemento en el centro</v-col>
    </v-row>
  </v-container>
</template>
```
## Flex Align

Las clases de "align" en Vuetify 3 te permiten controlar cómo se alinean los elementos dentro de un contenedor flex a lo largo del eje transversal. Estas clases afectan la alineación vertical de los elementos.

- `.align-{value}`: Controla la alineación en todos los tamaños de pantalla.
- `.align-{breakpoint}-{value}`: Controla la alineación en un breakpoint específico.

Valores de alineación disponibles:

- `start`: Alinea los elementos al principio del eje transversal.
- `end`: Alinea los elementos al final del eje transversal.
- `center`: Alinea los elementos en el centro del eje transversal.
- `baseline`: Alinea los elementos en su línea de base.
- `stretch`: Estira los elementos para que ocupen todo el espacio disponible en el eje transversal.

Ejemplo de uso de clases de alineación flex en Vuetify:

```vue
<template>
  <v-container>
    <v-row class="align-start">
      <v-col>Elemento al principio</v-col>
      <v-col>Elemento al principio</v-col>
    </v-row>
    
    <v-row class="align-center">
      <v-col>Elemento en el centro</v-col>
      <v-col>Elemento en el centro</v-col>
    </v-row>
  </v-container>
</template>
```
## Flex Align Self

Las clases de "align-self" en Vuetify 3 te permiten controlar la alineación de elementos individuales dentro de un contenedor flex. Esto es útil cuando deseas que un elemento se alinee de manera diferente en relación con los otros elementos dentro del mismo contenedor flex.

- `.align-self-{value}`: Controla la alineación del elemento en todos los tamaños de pantalla.
- `.align-self-{breakpoint}-{value}`: Controla la alineación del elemento en un breakpoint específico.

Valores de alineación disponibles:

- `start`: Alinea el elemento al principio del eje transversal.
- `end`: Alinea el elemento al final del eje transversal.
- `center`: Alinea el elemento en el centro del eje transversal.
- `baseline`: Alinea el elemento en su línea de base.
- `stretch` o `auto`: Estira el elemento para que ocupe todo el espacio disponible en el eje transversal.

Ejemplo de uso de clases de alineación individual en Vuetify:

```vue
<template>
  <v-container>
    <v-row>
      <v-col class="align-self-start">Este elemento se alinea arriba</v-col>
      <v-col class="align-self-center">Este elemento se alinea en el centro</v-col>
    </v-row>
  </v-container>
</template>
```
### Flex Wrap

Las clases de "flex wrap" en Vuetify 3 te permiten controlar cómo los elementos se envuelven dentro de un contenedor flex cuando no caben en el espacio disponible. Puedes usar las siguientes clases para lograr esto:

- `.flex-{value}`: Controla el comportamiento de envoltura en todos los tamaños de pantalla.
- `.flex-{breakpoint}-{value}`: Controla el comportamiento de envoltura en un breakpoint específico.

**Valores de envoltura disponibles:**

- `nowrap`: Los elementos no se envuelven y se superponen si no caben.
- `wrap`: Los elementos se envuelven a la siguiente línea si no caben en el espacio disponible.
- `wrap-reverse`: Los elementos se envuelven a la siguiente línea en orden inverso si no caben.

#### Ejemplo de uso en Vuetify:

```vue
<template>
  <v-container>
    <v-row class="flex-wrap">
      <v-col>
        Elemento 1
      </v-col>
      <v-col>
        Elemento 2
      </v-col>
      <v-col>
        Elemento 3
      </v-col>
    </v-row>
  </v-container>
</template>
```
### Flex Order

Las clases de "flex order" en Vuetify 3 te permiten controlar el orden de visualización de elementos dentro de un contenedor flex sin cambiar el orden en el código fuente. Puedes usar las siguientes clases para lograr esto:

- `.order-{value}`: Controla el orden en todos los tamaños de pantalla.
- `.order-{breakpoint}-{value}`: Controla el orden en un breakpoint específico.

**Valores de orden disponibles:**

- `first`: Coloca el elemento al principio.
- `last`: Coloca el elemento al final.
- Números del `0` al `12`: Controla el orden numéricamente, donde un número menor se muestra antes.

#### Ejemplo de uso en Vuetify:

```vue
<template>
  <v-container>
    <v-row>
      <v-col class="order-first">Elemento al principio</v-col>
      <v-col class="order-last">Elemento al final</v-col>
      <v-col class="order-2">Elemento 2do en orden</v-col>
    </v-row>
  </v-container>
</template>
```
### Flex Align Content

Las clases de "align content" en Vuetify 3 te permiten controlar la alineación del contenido dentro de un contenedor flex cuando hay espacio adicional en el eje transversal. Puedes usar las siguientes clases para lograr esto:

- `.align-content-{value}`: Controla la alineación del contenido en todos los tamaños de pantalla.
- `.align-{breakpoint}-content-{value}`: Controla la alineación del contenido en un breakpoint específico.

**Valores de alineación disponibles:**

- `start`: Alinea el contenido al principio del eje transversal.
- `end`: Alinea el contenido al final del eje transversal.
- `center`: Alinea el contenido en el centro del eje transversal.
- `space-between`: Distribuye uniformemente el espacio entre el contenido.
- `space-around/stretch`: Distribuye uniformemente el espacio alrededor del contenido y estira el contenido para ocupar el espacio disponible.

#### Ejemplo de uso en Vuetify:

```vue
<template>
  <v-container>
    <v-row class="align-content-start">
      <v-col>Contenido al principio</v-col>
      <v-col>Contenido al principio</v-col>
    </v-row>
    
    <v-row class="align-content-space-between">
      <v-col>Contenido con espacio entre</v-col>
      <v-col>Contenido con espacio entre</v-col>
    </v-row>
  </v-container>
</template>
```
### Flex Grow and Shrink

Las clases de "flex grow and shrink" en Vuetify 3 te permiten controlar el comportamiento de crecimiento y contracción de elementos dentro de un contenedor flex en función de ciertas condiciones. Puedes usar las siguientes clases para lograr esto:

- `flex-{breakpoint}-{condition}-{state}`: Controla el comportamiento en un breakpoint específico.

**Condiciones disponibles:**

- `grow`: Controla el crecimiento de un elemento.
- `shrink`: Controla la contracción de un elemento.

**Estados disponibles:**

- `0`: Desactiva el crecimiento o la contracción del elemento.
- `1`: Activa el crecimiento o la contracción del elemento.

#### Ejemplo de uso en Vuetify:

```vue
<template>
  <v-container>
    <v-row>
      <v-col class="flex-md-grow-1">Elemento que crece en pantallas medianas o más grandes</v-col>
      <v-col class="flex-shrink-0">Elemento que no se contrae</v-col>
    </v-row>
  </v-container>
</template>
```
### Float

Las clases de "float" en Vuetify 3 te permiten controlar la posición de un elemento dentro de su contenedor. Puedes usar las siguientes clases para lograr esto:

- `.float-{value}`: Controla la posición en todos los tamaños de pantalla.
- `.float-{breakpoint}-{value}`: Controla la posición en un breakpoint específico.

**Valores disponibles:**

- `left`: Coloca el elemento a la izquierda del contenedor.
- `right`: Coloca el elemento a la derecha del contenedor.
- `none`: Restaura la posición predeterminada del elemento.

#### Ejemplo de uso en Vuetify:

```vue
<template>
  <v-container>
    <v-row>
      <v-col class="float-left">Elemento flotante a la izquierda</v-col>
      <v-col class="float-right">Elemento flotante a la derecha</v-col>
    </v-row>
  </v-container>
</template>
```
### Spacing

Las clases de "spacing" en Vuetify 3 te permiten controlar el espacio (margen o relleno) alrededor de un elemento. Puedes usar las siguientes clases para lograr esto:

- `.{property}{direction}-{size}`: Controla el espacio para margen (m) o relleno (p) en una dirección específica y con un tamaño determinado.

**Propiedades disponibles:**

- `m`: Aplica margen.
- `p`: Aplica relleno.

**Direcciones disponibles:**

- `t`: Aplica el espacio en la parte superior (margen o relleno).
- `b`: Aplica el espacio en la parte inferior (margen o relleno).
- `l`: Aplica el espacio en la parte izquierda (margen o relleno).
- `r`: Aplica el espacio en la parte derecha (margen o relleno).
- `s`: Aplica el espacio en la parte izquierda (en modo LTR) o la parte derecha (en modo RTL) (margen o relleno).
- `e`: Aplica el espacio en la parte derecha (en modo LTR) o la parte izquierda (en modo RTL) (margen o relleno).
- `x`: Aplica el espacio en la parte izquierda y derecha (margen o relleno).
- `y`: Aplica el espacio en la parte superior e inferior (margen o relleno).
- `a`: Aplica el espacio en todas las direcciones (margen o relleno).

**Tamaños disponibles:**

- `0`: Establece el margen o relleno en 0.
- `1`: Establece el margen o relleno en 4px.
- `2`: Establece el margen o relleno en 8px.
- `3`: Establece el margen o relleno en 12px.
- `4`: Establece el margen o relleno en 16px.
- `5`: Establece el margen o relleno en 20px.
- `6`: Establece el margen o relleno en 24px.
- `7`: Establece el margen o relleno en 28px.
- `8`: Establece el margen o relleno en 32px.
- `9`: Establece el margen o relleno en 36px.
- `10`: Establece el margen o relleno en 40px.
- `11`: Establece el margen o relleno en 44px.
- `12`: Establece el margen o relleno en 48px.
- `13`: Establece el margen o relleno en 52px.
- `14`: Establece el margen o relleno en 56px.
- `15`: Establece el margen o relleno en 60px.
- `16`: Establece el margen o relleno en 64px.
- `n1`: Establece el margen en -4px.
- `n2`: Establece el margen en -8px.
- `n3`: Establece el margen en -12px.
- `n4`: Establece el margen en -16px.
- `n5`: Establece el margen en -20px.
- `n6`: Establece el margen en -24px.
- `n7`: Establece el margen en -28px.
- `n8`: Establece el margen en -32px.
- `n9`: Establece el margen en -36px.
- `n10`: Establece el margen en -40px.
- `n11`: Establece el margen en -44px.
- `n12`: Establece el margen en -48px.
- `n13`: Establece el margen en -52px.
- `n14`: Establece el margen en -56px.
- `n15`: Establece el margen en -60px.
- `n16`: Establece el margen en -64px.
- `auto`: Establece el margen en automático.

#### Ejemplo de uso en Vuetify:

```vue
<template>
  <v-container>
    <v-row>
      <v-col class="m-t-2">Margen en la parte superior de 8px</v-col>
      <v-col class="p-x-3">Relleno en la parte izquierda y derecha de 12px</v-col>
    </v-row>
  </v-container>
</template>
```
### Typography

Las clases de "typography" en Vuetify 3 te permiten controlar la tipografía y el estilo del texto en tus elementos. Puedes usar las siguientes clases para lograr esto:

- `.text-{value}`: Controla el estilo del texto en todos los tamaños de pantalla.
- `.text-{breakpoint}-{value}`: Controla el estilo del texto en un breakpoint específico.

**Valores disponibles:**

- `h1`: Establece el tamaño de fuente en 6rem y el peso de fuente en 300.
- `h2`: Establece el tamaño de fuente en 3.75rem y el peso de fuente en 300.
- `h3`: Establece el tamaño de fuente en 3rem y el peso de fuente en 400.
- `h4`: Establece el tamaño de fuente en 2.125rem y el peso de fuente en 400.
- `h5`: Establece el tamaño de fuente en 1.5rem y el peso de fuente en 400.
- `h6`: Establece el tamaño de fuente en 1.25rem y el peso de fuente en 500.
- `subtitle-1`
- `subtitle-2`
- `body-1`
- `body-2`
- `button`
- `caption`
- `overline`

#### Ejemplo de uso en Vuetify:

```vue
<template>
  <v-container>
    <v-row>
      <v-col class="text-h1">Título de Nivel 1</v-col>
      <v-col class="text-body-1">Cuerpo de Texto 1</v-col>
    </v-row>
  </v-container>
</template>
```
### Text Alignment

Las clases de "text alignment" en Vuetify 3 te permiten controlar la alineación del texto dentro de elementos. Puedes usar las siguientes clases para lograr esto:

- `.text-{value}`: Controla la alineación del texto en todos los tamaños de pantalla.
- `.text-{breakpoint}-{value}`: Controla la alineación del texto en un breakpoint específico.

**Valores de alineación disponibles:**

- `left`: Alinea el texto a la izquierda.
- `center`: Alinea el texto en el centro.
- `right`: Alinea el texto a la derecha.

#### Ejemplo de uso en Vuetify:

```vue
<template>
  <v-container>
    <v-row>
      <v-col class="text-left">Texto alineado a la izquierda</v-col>
      <v-col class="text-center">Texto centrado</v-col>
      <v-col class="text-right">Texto alineado a la derecha</v-col>
    </v-row>
  </v-container>
</template>
```
### Text Decoration

Las clases de "text decoration" en Vuetify 3 te permiten controlar la decoración del texto en tus elementos. Puedes usar las siguientes clases para lograr esto:

- `text-decoration-none`: Elimina cualquier decoración de texto.
- `text-decoration-overline`: Agrega una línea sobre el texto.
- `text-decoration-underline`: Agrega una línea debajo del texto.
- `text-decoration-line-through`: Agrega una línea a través del texto.

#### Ejemplo de uso en Vuetify:

```vue
<template>
  <v-container>
    <v-row>
      <v-col class="text-decoration-none">Texto sin decoración</v-col>
      <v-col class="text-decoration-overline">Texto con línea superior</v-col>
      <v-col class="text-decoration-underline">Texto con línea inferior</v-col>
      <v-col class="text-decoration-line-through">Texto con línea a través</v-col>
    </v-row>
  </v-container>
</template>
```
### Text Wrapping and Overflow

Las clases de "text wrapping and overflow" en Vuetify 3 te permiten controlar cómo se envuelve el texto y cómo se maneja el desbordamiento del texto en tus elementos. Puedes usar las siguientes clases para lograr esto:

- `.text-wrap`: Evita que el texto se divida en varias líneas.
- `.text-no-wrap`: Evita que el texto se divida en varias líneas.
- `.text-truncate`: Evita que el texto se divida en varias líneas y muestra puntos suspensivos (...) cuando el texto se desborda.
- `.text-break`: Permite que el texto se divida en varias líneas y ajusta automáticamente el texto para evitar desbordamiento.

#### Ejemplo de uso en Vuetify:

```vue
<template>
  <v-container>
    <v-row>
      <v-col class="text-wrap">Este es un texto largo que no se dividirá en varias líneas y se desplazará horizontalmente si es necesario.</v-col>
      <v-col class="text-truncate">Este es otro texto largo que mostrará puntos suspensivos si se desborda...</v-col>
      <v-col class="text-break">Este texto se dividirá en varias líneas si es necesario y se ajustará automáticamente.</v-col>
    </v-row>
  </v-container>
</template>
```
### Text Transform

Las clases de "text transform" en Vuetify 3 te permiten controlar la transformación del texto en tus elementos. Puedes usar las siguientes clases para lograr esto:

- `text-none`: No aplica ninguna transformación al texto.
- `text-lowercase`: Convierte el texto en minúsculas.
- `text-uppercase`: Convierte el texto en mayúsculas.
- `text-capitalize`: Capitaliza la primera letra de cada palabra.

#### Ejemplo de uso en Vuetify:

```vue
<template>
  <v-container>
    <v-row>
      <v-col class="text-none">Texto sin transformación</v-col>
      <v-col class="text-lowercase">texto en minúsculas</v-col>
      <v-col class="text-uppercase">TEXTO EN MAYÚSCULAS</v-col>
      <v-col class="text-capitalize">Texto Capitalizado</v-col>
    </v-row>
  </v-container>
</template>
```
### Text Opacity

Las clases de "text opacity" en Vuetify 3 te permiten controlar la opacidad del texto en tus elementos para diferentes estados. Puedes usar las siguientes clases para lograr esto:

- `text--primary`: Establece la opacidad del texto al 87% para el estado primario.
- `text--secondary`: Establece la opacidad del texto al 60% para el estado secundario.
- `text--disabled`: Establece la opacidad del texto al 37% para el estado deshabilitado.

#### Ejemplo de uso en Vuetify:

```vue
<template>
  <v-container>
    <v-row>
      <v-col class="text--primary">Texto en estado primario</v-col>
      <v-col class="text--secondary">Texto en estado secundario</v-col>
      <v-col class="text--disabled">Texto en estado deshabilitado</v-col>
    </v-row>
  </v-container>
</template>
```
### Font Weights

Las clases de "font weights" en Vuetify 3 te permiten controlar el peso de la fuente en tus elementos. Puedes usar las siguientes clases para lograr esto:

- `font-weight-thin`: Establece el peso de la fuente en 100.
- `font-weight-light`: Establece el peso de la fuente en 300.
- `font-weight-regular`: Establece el peso de la fuente en 400.
- `font-weight-medium`: Establece el peso de la fuente en 500.
- `font-weight-bold`: Establece el peso de la fuente en 700.
- `font-weight-black`: Establece el peso de la fuente en 900.

#### Ejemplo de uso en Vuetify:

```vue
<template>
  <v-container>
    <v-row>
      <v-col class="font-weight-thin">Texto con peso de fuente delgado</v-col>
      <v-col class="font-weight-regular">Texto con peso de fuente regular</v-col>
      <v-col class="font-weight-bold">Texto con peso de fuente en negrita</v-col>
    </v-row>
  </v-container>
</template>
```
