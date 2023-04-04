# ler-valores
class Program
{
    static void Main(string[] args)
    {
        double[] numeros = new double[6];
        int positivos = 0;
        double somaPositivos = 0;



        for (int i = 0; i < 6; i++)
        {
            numeros[i] = double.Parse(Console.ReadLine());

            if (numeros[i] > 0)
            {
                positivos++;
                somaPositivos += numeros[i];
            }
        }

        Console.WriteLine(positivos + " valores positivos");

        if (positivos > 0)
        {
            double mediaPositivos = somaPositivos / positivos;
            Console.WriteLine(mediaPositivos.ToString("F1"));
        }

    }
}
