```cs
class Result
{

    public static void solve(double meal_cost, int tip_percent, int tax_percent)
    {
        double tip = meal_cost * tip_percent / 100;
        double tax = tax_percent * meal_cost / 100;
        double total_cost = meal_cost + tip + tax;
        
        Console.WriteLine(Math.Round(total_cost));
    }

}

class Solution
{
    public static void Main(string[] args)
    {
        double meal_cost = Convert.ToDouble(Console.ReadLine().Trim());

        int tip_percent = Convert.ToInt32(Console.ReadLine().Trim());

        int tax_percent = Convert.ToInt32(Console.ReadLine().Trim());

        Result.solve(meal_cost, tip_percent, tax_percent);
    }
}
```
