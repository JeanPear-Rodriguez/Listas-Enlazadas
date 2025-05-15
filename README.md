<?php 


clases Nodo{
     Public $dato;
     Public $siguiente;
       public función _construct($dato)  {
           $This ->dato = $dato;
           $This ->siguiente = null;
      }
}

Clases ListaEnlazada{
        Public $cabeza;
        Public función _ construct (){
           $This ->cabeza = null;
        }
  
 Public función insertar ($dato){
      $nuevoNodo = new Nodo($dato)
      $nuevoNodo ->siguiente=$this->cabeza;
      $this->cabeza=$nuevoNodo;
}
 Public función IMPRIMIR HTML () {
    $actual = $this->cabeza;
    echo"<ul>" ;

   While($actual!=null){
   echo "<li>" . $actual->dato."</li>" ;
   $actual= $actual->siguiente ;
}

 echo"</ul>" ;

$lista = new Listas enlazada () ;

$Lista->insertar("Ferrari") ;
$Lista->insertar("Lamborgini") ;
$Lista->insertar("Pagani") ;
$Lista->imprimirHTML () ; 

?>
