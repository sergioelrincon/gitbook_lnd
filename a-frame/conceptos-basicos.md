# Conceptos básicos

## Conceptos Básicos de A-Frame

A-Frame es una poderosa herramienta que nos permite crear experiencias de realidad virtual (VR) en la web utilizando un enfoque similar al HTML. Al adentrarnos en A-Frame, es crucial entender tres conceptos fundamentales: entidades, componentes y sistemas. Estos conceptos forman la base de cómo A-Frame organiza y maneja escenarios 3D y experiencias VR.

### **Entidades, Componentes y Sistemas**

* **Entidades:** En A-Frame, una entidad es un objeto general que puede ser cualquier cosa dentro de una escena, desde objetos visibles como luces y modelos 3D, hasta conceptos abstractos como controles de cámara. Las entidades se representan con el elemento `<a-entity>` y funcionan como contenedores que pueden llevar uno o más componentes. Puedes pensar en una entidad como un "div" en HTML, pero para el mundo 3D.
* **Componentes:** Los componentes son módulos reutilizables que se adjuntan a las entidades para proporcionarles apariencia, comportamiento y funcionalidad. Por ejemplo, un componente puede definir cómo se ve un objeto (color, textura), cómo se mueve o cómo interactúa con el usuario. Cada entidad puede tener múltiples componentes, lo que permite una gran flexibilidad y reutilización. Los componentes en A-Frame son equivalentes a las propiedades CSS en el desarrollo web tradicional, pero con la capacidad de influir en el comportamiento y las interacciones 3D, además de la apariencia.
* **Sistemas:** Los sistemas en A-Frame proporcionan la lógica global que puede afectar a múltiples entidades y componentes. Funcionan en el nivel más alto, controlando complejos comportamientos y coordinaciones entre varios componentes. Un sistema podría, por ejemplo, gestionar cómo todos los objetos de una determinada clase reaccionan a un evento específico. Piensa en los sistemas como en JavaScript, que actúa sobre múltiples elementos HTML en una página web, pero en este caso, para gestionar y coordinar comportamientos en un entorno 3D.

### **Escena en A-Frame**

El elemento `<a-scene>` es el contenedor principal de cualquier proyecto A-Frame. Actúa como el lienzo sobre el cual se dibujan todos nuestros objetos 3D, luces y cámaras. Este elemento configura el entorno, manejando cosas como la renderización, la cámara, la iluminación básica, y más. Al igual que el elemento "body" en HTML, `<a-scene>` contiene todos los objetos y entidades que componen tu experiencia VR o 3D.

### **Creación de Objetos 3D Básicos**

A-Frame simplifica la creación de objetos 3D mediante el uso de "primitivas". Estas primitivas son entidades predefinidas que representan formas geométricas básicas como cajas (`<a-box>`), esferas (`<a-sphere>`), cilindros (`<a-cylinder>`), y planos (`<a-plane>`). Cada una de estas entidades ya viene con componentes estándar para definir su geometría, material, posición, rotación, y escala. Modificar estas entidades es tan sencillo como cambiar los atributos HTML, lo que permite a los desarrolladores y diseñadores crear y manipular objetos 3D sin necesidad de profundizar en complejas APIs de gráficos 3D.

### **Importancia del Sistema de Coordenadas**

En A-Frame, el posicionamiento y la orientación de las entidades dentro de la escena se gestionan a través de un sistema de coordenadas 3D, donde cada punto en el espacio se define por tres valores: X (horizontal), Y (vertical) y Z (profundidad). Este sistema es esencial para colocar, rotar, y escalar objetos en tu escena de manera precisa. Manipular estas propiedades permite a los diseñadores y desarrolladores organizar el layout de sus experiencias VR de una forma intuitiva y visual.

### **Inspeccionar y Modificar Escenas en Tiempo Real**

Una herramienta invaluable en el desarrollo con A-Frame es el inspector. Este se puede activar en cualquier escena A-Frame presionando `Ctrl + Alt + I` en el navegador. El inspector permite a los desarrolladores y diseñadores ver y modificar la escena en tiempo real, proporcionando una forma

## Ejemplo

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title>A-Frame Scene Example</title>
    <script src="https://aframe.io/releases/1.2.0/aframe.min.js"></script>
</head>
<body>
    <!-- A-Frame scene: contenedor principal donde se monta nuestra experiencia VR -->
    <a-scene>
        <!-- Cámara: define el punto de vista del usuario en la escena -->
        <a-camera position="0 1.6 0"></a-camera>
        
        <!-- Luz ambiental: ilumina todos los objetos de manera uniforme -->
        <a-light type="ambient" color="#fff"></a-light>
        
        <!-- Luz direccional: simula luz solar para generar sombras -->
        <a-light type="directional" position="-2 4 -5" intensity="0.5"></a-light>
        
        <!-- Primitiva caja: objeto 3D básico con posición, rotación y color -->
        <a-box position="-1 0.5 -3" rotation="0 45 0" color="#4CC3D9"></a-box>
        
        <!-- Primitiva esfera: otro objeto 3D básico, con diferentes atributos -->
        <a-sphere position="1 0.5 -3" radius="0.5" color="#EF2D5E"></a-sphere>
        
        <!-- Primitiva cilindro: demostración de una forma 3D más, con textura -->
        <a-cylinder position="0 0.75 -5" radius="0.5" height="1.5" color="#FFC65D"></a-cylinder>
        
        <!-- Entidad compuesta equivalente a una primitiva: un toroide hecho de entidades básicas -->
        <!-- Este bloque demuestra cómo combinar entidades básicas para formar objetos complejos -->
        <a-entity position="3 0.5 -5">
            <a-torus color="#7BC8A4" radius="1" radius-tubular="0.1"></a-torus>
        </a-entity>
        
        <!-- Plano: sirve como suelo para la escena -->
        <a-plane position="0 0 -4" rotation="-90 0 0" width="10" height="10" color="#7DA7D9"></a-plane>
        
        <!-- Sistema de coordenadas explicado en comentarios -->
        <!-- X positivo a la derecha, Y positivo hacia arriba, Z positivo sale de la pantalla -->
    </a-scene>
</body>
</html>

```
