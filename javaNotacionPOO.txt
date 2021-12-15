
package com.ejemploJava;
 
/*Ejemplo de como crear una clase en Java*/
public class Telefono {
//Encapsulamiento : 
 private String marca;//Modificador private
 public int capacidad;//Modificador public
 protected String modelo; //Modificador protected
 
/*Acceder a los atributos de nuestra clase atraves de los getters y setters y no tocarlos directamente*/
 public void setMarca(String marca) {
   this.marca = marca;
 }
 public int getCapacidad() {
   return capacidad;
 }
 public void setCapacidad(int capacidad) {
   this.capacidad = capacidad;
 }
 
/*Constructor*/
 public Telefono(String marca, int capacidad) {
   super();
   this.marca = marca;
   this.capacidad = capacidad;
 }
 
/*Métodos/Funciones que puede tener nuestra clase a los cuales luego podemos llamar a través de los objetos que instanciamos de la clase*/
  public int duracionBateria() {
  
   if (capacidad<3000) {
     return 16;
   }else {
    
     return 24;
   }
 }