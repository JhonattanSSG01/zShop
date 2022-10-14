# Bienvenidos a zShop 👋👋‼
![image](https://user-images.githubusercontent.com/80645321/195891907-cd423d3e-47aa-40fa-99fa-b9be2f63f77e.png)
Puedes visitarla en el sigiuiente link 👉 https://jhonattanssg01.github.io/zShop/

# Inicio Del Proyecto 💢
> Primordialmente se realizó un fork al repositorio de Jimmy, donde se encontraba todo lo relacionado con el proyecto de zShop, se hizo este método para tener una copia de ese repositorio en un nuevo repositorio pero en mi GitHub. Gracias a esto, podemos dar Git push sin afectar el repositorio original. Finalmente lo clone en local para poder trabajar.
>### 	El comando en Git para clonar el repositorio es $ git clone <URL del repositorio a clonar> 📥

Luego de revisar la estructura de la web, logre entender cuales etiquetas, clases y id hacian referencia para poder modificar la estructura con lo planteado en el trello.

# Nuevos estilos CSS agregados 💯
## Contenedor principal (body)🔲

```
/* Estilos vista Index */
/* Estilos body */
.wrap-body{
  display: flex;
  flex-direction: column;
  align-items: center;
}

.zerogrid{
  width: 1000px;
}
```
Prácticamente en esta parte de los estilos, se modificó la parte que contiene todo el contenido principal para qué se adaptará mucho mejor al centro con un ancho establecido.  

## Contenedor Encabezado (header)⬜
```
/* Estilos header */
.main-header .row{
  display: flex;
  justify-content: space-between;
  align-items: center;
}
```
En esta parte de los estilos, se modificó la parte superior que contiene el logo y el menú para lograr una alineación y espaciado entre ellos visualizándose conjuntamente en la misma fila.  

## Contendor de la caja #2⬛
```
<div class="grid-principal">
	<div class="col-2-5 box-item">
		<a class="box-item-inner" href="#">
      'Etiquetas correspondientes de cada caja'
		</a>
	</div>
</div>
```
En esta parte del código altere un poco el HTML para poder alinear cada cajita en una cuadricula, lo que se hizo fue poner los div con clase ="box-item" dentro de un div para poder usar acorde la cuadricula en el CSS.

```
/* Estilos content-box2 */

.content-box.box-2 >.wrap-box{
  display: grid;
  grid-template-columns: 40% 10% 10% 40%;
  grid-template-rows: repeat(3, 300px);
}
                                                
.grid-principal{
  grid-area: 1 / 1 / 2 / 2;
}
```
En esta parte de los estilos, se agregó una cuadrícula para acomodar favorablemente y acorde al tamaño de cada caja de contenido dentro de un contenedor global para lograr una mejor visualización.

## Contenedor de la caja #3🔳
```
/* Estilos content-box3 */
.content-box.box-3 >.row.wrap-box{
  display: grid;
  grid-template-columns: 50%;
}
```
En esta parte de los estilos, se agregó una cuadrícula básica para acomodar en dos columnas información primordial y que no se sobrepusiera sobre otro elemento.

## Contenedor pie de página(footer)🔘🔘
```
/* Estilos footer */
.wrap-footer >.row{
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}
```
En esta parte de los estilos, se agregó una cuadrícula básica de tres columnas para alinear mejor el contenido de cada mini seccion dentro del footer.

## Vista single➰
```

/* Estilos vista single */
.single-post >.row.wrap-post{
  margin: 0;
}
```
En esta parte de los estilos, se modifico el espaciado entre el contenedor del header y body. 

## Vista About➰
```
/* Estilos vista about */
.row.wrap-post >.flex-box{
  display: grid;
  grid-template-columns: repeat(2, 1fr);
}
```
En esta parte de los estilos, se agregó un cuadricula básica para alinear el contenido en dos columnas y se logrará visualizar las imagenes con su respectiva descripción.

## Vista contact➰
```
/* Estilos vista contact */
.t-center{
  margin: 0;
  padding: 50px;
}

form .row:first-child{
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 15px;
}
```
En esta ultima parte de los estilos, se agregó un cuadricula para alinear el contenido en dos columnas y se logrará visualizar los campos de texto mucho mejor.Además, se altero el espaciado entre el contenedor header y body.
