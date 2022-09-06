    public static void main(String[] args) {
        // TODO code application logic here
        Scanner leer = new Scanner(System.in);
        System.out.print("Ingrese el numero de horas trabajadas en la semana: ");
        int h_trabajo = leer.nextInt();
        int horas_extra;
        int pago_extra;
        int tarifa;
        int sueldo_total;
        int horas;
        
        if (h_trabajo <= 40)
        {
            tarifa = h_trabajo * 20;
            System.out.print("Su tarifa de pago es: $"+ tarifa);
        }
        if (h_trabajo > 40)
        {
            horas_extra = h_trabajo - 40;
            pago_extra = horas_extra*25;
            horas = h_trabajo - horas_extra;
            sueldo_total = (horas * 20)+(pago_extra);
            System.out.println("Su tarifa de pago es: $"+ sueldo_total);
        }
    }
}
