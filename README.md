# Proyecto-integrador-2do
leo -anibal-jeni-ariel

package singer;

import java.util.Scanner;


public class Singer {

   
    public static void main(String[] args) {
        String Nombre_del_cliente; float valor_orden; boolean pagado;boolean abonado;boolean no_pagado;
            Scanner ing=new Scanner(System.in);
            cliente client = new cliente();
               
    }
 //anibal es guapo y maricon    
}



//clases editar 


package singer;


 public class servicio extends cliente {
    private String Nombre_del_servicio;
    private float Precio_unitario;
    private int Codigo;
    private float precio_total;
    public servicio(String Nombre_del_servicio, float Precio_unitario, int Codigo, float precio_total, String Nombre_del_cliente, float         valor_orden, boolean pagado, boolean abonado, boolean no_pagado) {
        super(Nombre_del_cliente, valor_orden, pagado, abonado, no_pagado);
        this.Nombre_del_servicio = Nombre_del_servicio;
        this.Precio_unitario = Precio_unitario;
        this.Codigo = Codigo;
        this.precio_total = precio_total;
    }

    public String getNombre_del_servicio() {
        return Nombre_del_servicio;
    }

    public void setNombre_del_servicio(String Nombre_del_servicio) {
        this.Nombre_del_servicio = Nombre_del_servicio;
    }

    public float getPrecio_unitario() {
        return Precio_unitario;
    }

    public void setPrecio_unitario(float Precio_unitario) {
        this.Precio_unitario = Precio_unitario;
    }

    public int getCodigo() {
        return Codigo;
    }

    public void setCodigo(int Codigo) {
        this.Codigo = Codigo;
    }

    public float getPrecio_total() {
        return precio_total;
    }

    public void setPrecio_total(float precio_total) {
        this.precio_total = precio_total;
    }

}

class asesoramiento extends servicio{
    private float precio_por_la_asesoria;

    public asesoramiento(float precio_por_la_asesoria, String Nombre_del_servicio, float Precio_unitario, int Codigo, float precio_total, String Nombre_del_cliente, float valor_orden, boolean pagado, boolean abonado, boolean no_pagado) {
        super(Nombre_del_servicio, Precio_unitario, Codigo, precio_total, Nombre_del_cliente, valor_orden, pagado, abonado, no_pagado);
        this.precio_por_la_asesoria = precio_por_la_asesoria;
    }

    public float getPrecio_por_la_asesoria() {
        return precio_por_la_asesoria;
    }

    public void setPrecio_por_la_asesoria(float precio_por_la_asesoria) {
        this.precio_por_la_asesoria = precio_por_la_asesoria;
    }
    
    
}


//clases editar 

package singer;

public class cliente {
   private String Nombre_del_cliente;
   private float valor_orden;
   private boolean pagado;
   private boolean abonado;
   private boolean no_pagado;

    public cliente(String Nombre_del_cliente, float valor_orden, boolean pagado, boolean abonado, boolean no_pagado) {
        this.Nombre_del_cliente = Nombre_del_cliente;
        this.valor_orden = valor_orden;
        this.pagado = pagado;
        this.abonado = abonado;
        this.no_pagado = no_pagado;
    }

    cliente() {
        throw new UnsupportedOperationException("Not supported yet."); //To change body of generated methods, choose Tools | Templates.
    }

    public String getNombre_del_cliente() {
        return Nombre_del_cliente;
    }

    public void setNombre_del_cliente(String Nombre_del_cliente) {
        this.Nombre_del_cliente = Nombre_del_cliente;
    }

    public float getValor_orden() {
        return valor_orden;
    }

    public void setValor_orden(float valor_orden) {
        this.valor_orden = valor_orden;
    }

    public boolean isPagado() {
        return pagado;
    }

    public void setPagado(boolean pagado) {
        this.pagado = pagado;
    }

    public boolean isAbonado() {
        return abonado;
    }

    public void setAbonado(boolean abonado) {
        this.abonado = abonado;
    }

    public boolean isNo_pagado() {
        return no_pagado;
    }

    public void setNo_pagado(boolean no_pagado) {
        this.no_pagado = no_pagado;
    }

}

