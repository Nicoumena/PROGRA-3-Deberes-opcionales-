public class Carros {
         private int codigo;       // Identificador único de 3 cifras
         private String marca;     //
         private int cilindraje;   //
         private double precio;     //

    public Carros (int codigo, String marca, int cilindraje, String color, double precio) {
        this.codigo = codigo;
        this.marca = marca;
        this.cilindraje = cilindraje;
        this.precio = precio;
    }

    public int getCodigo() {
        return codigo;
    }

    public void setCodigo(int codigo) {
        if (codigo>=100 && codigo<=999) {

            this.codigo = codigo;
        }else {
            throw  new IllegalArgumentException("El codigo debe tener tres digitos");
        }



    }


    public String getMarca() {
        return marca;
    }

    public void setMarca(String marca) {
        this.marca = marca;
    }

    public int getCilindraje() {
        return cilindraje;
    }

    public void setCilindraje(int cilindraje) {
        this.cilindraje = cilindraje;
    }

    public double getPrecio() {
        return precio;
    }

    public void setPrecio(double precio) {
        if (precio>5000 && precio<100000) {

        this.precio = precio;
    }else {
            throw  new IllegalArgumentException("El precio debe estar entre 5000 y 100 000");
        }



    }
}
