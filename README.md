public class primos{
public static boolean primo (int nro)
{
    boolean dividiu=false;
    
    for (int i=2; i<nro; i++)
    {
        if (nro%i==0)
        {
            dividiu=true;
        }
    }
    return (!dividiu);
}
public static void main ()
{
    int qt=10, cont=1;
    while (qt>0)
    {
        cont++;
        if (primo(cont))
        {
            System.out.println(cont);
            qt--;
        }
    }
}
}
