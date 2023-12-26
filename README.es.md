<h1>CSS USEFUL LINES</h1>

Tus proyectos apestan, y lo van a seguir haciendo hasta que corrijas lo que te voy a mostrar acá.

Cada navegador se encarga de hacer lo que le plazca con aquellas cosas que no le especificás cómo querés que sean. 

Hay detalles que sólo los sufren los clientes; no vos, desarrollador.

<hr/>
<h2>Index</h2>

* [Estilar la Barra de Scroll](#scroll)

* [Quitar efectos en Dispositivos Mobiles](#toucheffect)

* [Quitar Flechitas del Input Number](#inputnum)

* [Te regalo unos Atajos](#snippets)

<hr/>
<h3 id="scroll">Estilar la Barra de Scroll</h3>

Ancho de la barra de scroll
```css
selector::-webkit-scrollbar {
    width: 10px;
}
```

Color del contenedor de la barra de scroll
```css   
body {
    scrollbar-color: gray;
}

body::-webkit-scrollbar-track {
    background: gray;
}
```


Estilos de la barra de scroll (la de adentro)
```css
body::-webkit-scrollbar-thumb {
    background-color: white; 
    border-radius: 10px; 
    border: 1px solid black; 
    padding: 5px;
}
```

<hr/>
<h3 id="toucheffect">Quitar efectos en Dispositivos Mobiles</h3>


Quitar el efecto al tocar ciertos selectores
(evita que el contenedor se ponga azul al presionar enlaces, imagenes y botones)
```css
a, img, button {
    text-decoration: none;
    user-select: none;
    -webkit-tap-highlight-color: transparent;
}
```

<hr/>
<h3 id="inputnum">Quitar Flechitas del Input Number</h3>


Presiona
- `Ctrl + Shift + P`
- Luego en Snippets
- Luego en css.json (CSS)
- Y pega el contenido de css.json de este repositorio

<h3>YA PODÉS USAR LOS ATAJOS</h3>
- `scrollb`: Añade una barra de scroll sencilla oscura
- `lscrollb`: Añade una barra de scroll sencilla clara
- `numinp`: Quita las flechitas de los input de números
- `rmtap`: Quita el efecto al tocar en enlaces en dispositivos mobiles
