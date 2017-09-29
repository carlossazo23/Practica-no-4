# Practica-no-4
package org.eclipse.che.examples;

public class HelloWorld { public static void main(String... argvs) {

  Node a = new Node();
  a.setPropiedad("Gua");
  
  Node b = new Node();
  b.setPropiedad("Mex");
  a.setNext(b);
  
  Node c = new Node();
  c.setPropiedad("Usa");
  a.getNext().setNext(c);
  
  Node d = new Node();
  d.setPropiedad("Esp");
  a.getNext().getNext().setNext(d);
  
  
  
   System.out.println(a.getPropiedad());
   System.out.println(a.getNext().getPropiedad());
   System.out.println(a.getNext().getNext().getPropiedad());
   System.out.println(a.getNext().getNext().getNext().getNext().getPropiedad());
   
   
}
private static class Node{
    private String Propiedad; 
    private Node next; 
    
    private String getPropiedad(){
        return this.Propiedad;
    }
    private void setPropiedad(String Propiedad){
        this.Propiedad = Propiedad;
    }
    
    
    private Node getNext(){
        return this.next;
        
    }
    private void setNext(Node Next){
        this.next = next; 
        
    }
    
    
    
    lista.addFitst("Gua");
    lista.addFitst("MEX");
    lista.addFitst("USA");
    lista.addFitst("ESP");
    lista.addFitst("FRA");
    lista.addFitst("ITA");
    lista.addFitst("RUS");
    lista.addFitst("SUI");
    lista.addFitst("CHI");
    lista.addFitst("JAP");
    lista.addFitst("COL");
    
    
    String valor = lista.removeFirst();
    while(valor != null){
        System.out.println(valor);
        valor = lista.removerFirst();
    }
    
}
}

SinglyLikedList

package org.eclipse.che.examples; //Clase

public class SinglyLinkedList {

private static class Node{
    private String Propiedad; 
    private Node next; 
    
    private String getPropiedad(){
        return this.Propiedad;
    }
    private void setPropiedad(String Propiedad){
        this.Propiedad = Propiedad;
    }
    
    
    private Node getNext(){
        return this.next;
        
    }
    private void setNext(Node Next){
        this.next = next;             
        
    }   
        private Node head = null;
        private Node tail = null;
        private int size = 0;
        
        public int size(){
            return size;
        }
        
        public boolean isEmpety(){
            return size == 0; 
        }
        public String first(){
            if(isEmpety ()) return null;
            return tail.getPropiedad();
        }    
        
        public String last(){
            if(isEmpety()) return null;
            return tail.getPropiedad();
        }
        
        public void addfirst(String e){
          
          head = new Node(e, null); 
          if(size ==0)
            tail = head;
            size++;
        }
        
        public void addLast(String e){
            Node newest = new Node(e, null); 
            if(isEmpty())
                 head = newest; 
            else
                tail.setNexst(newest);
             tail = newest;
             size++;
        }
        
        public String first(){
            return this.head.getPropiedad()
        
          public void addfirst(String e){
          
          head = new Node(e, null); 
          if(size ==0)
            tail = head;
            size++;
        }
        
        public void addLast(String e){
            Node newest = new Node(e, null); 
            if(isEmpty())
                 head = newest; 
            else
                tail.setNexst(newest);
             tail = newest;
             size++;
        }
        
      
}
}
