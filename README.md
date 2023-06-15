
# Tarea ED04

Es un simple proyecto donde tenemos una cuenta de banco y podemos retirar e ingresar dinero en ella, el principal tema era documentar el codigo.
    
    public static void operativa_cuenta(float cantidad){
        CCuenta cuenta1 = new CCuenta("Antonio López","1000-2365-85-1230456789",2500,0);
        double saldoActual = cuenta1.estado();
        System.out.println("El saldo actual es: "+ saldoActual );

        try {
            cuenta1.retirar(2300);
        } catch (Exception e) {
            System.out.print("Fallo al retirar!");
        }
        try {
            System.out.println("Ingreso en cuenta");
            cuenta1.ingresar(695);
        } catch (Exception e) {
            System.out.print("Fallo al ingresar!");
        }
    }
{} En esta parte es donde se desarrolla gran parte del ejercicio, al iniciar el programa nos permitira ingresar o retirar dinero, en caso de que alguna de las operaciones fallen nos dara un error, tambien tenemos la posibilidad de ver nuestro saldo actual
