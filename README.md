#CSS USEFUL LINES

Your projects stink, and they’re going to keep stinking until you fix what I’m going to show you here.

Each browser takes it upon itself to do whatever it pleases with those things that you don’t specify how you want them to be.

There are details that only the clients suffer; not you, the developer.


##Index

* [Scroll Bar Styles](#scroll)

* [Touch Effect on Mobile](#toucheffect)

* [Input Number Details](#inputnum)

* [Get Snippets](#snippets)


<h3 id="scroll">Scroll Bar Styles</h3>

Scrollbar Width
```css
selector::-webkit-scrollbar {
    width: 10px;
}
```

Container Scrollbar Color
```css   
body {
    scrollbar-color: gray;
}

body::-webkit-scrollbar-track {
    background: gray;
}
```


Bar Styles
```css
body::-webkit-scrollbar-thumb {
    background-color: white; 
    border-radius: 10px; 
    border: 1px solid black; 
    padding: 5px;
}
```


<h3 id="toucheffect">Touch Effect on Mobile</h3>


Remove tap effect on mobile browser
```css
a, img, button {
    text-decoration: none;
    user-select: none;
    -webkit-tap-highlight-color: transparent;
}
```


<h3 id="inputnum">Input Number Details</h3>


Remove the Up/Down Arrow into Input Number
```css
input[type=number]::-webkit-inner-spin-button, 
input[type=number]::-webkit-outer-spin-button { 
  -webkit-appearance: none; 
  margin: 0; 
}

input[type=number] { 
    -moz-appearance:textfield; 
}
```


<h3 id="snippets">Get Snippets</h3>


- Press `Ctrl + Shift + P`
- Select "Snippets"
- Select "css.json (CSS)" file
- Paste the content of css.json (of this repository) there

###ENJOY THE SNIPPETS
- `scrollb`: Scrollbar Styles Base Dark
- `lscrollb`: Scrollbar Styles Base Light
- `numinp`: Remove Up/Down Arrows into Input Number
- `rmtap`: Remove Tap Effect
