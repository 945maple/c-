c%
主要记录自己学习c#各个知识点练习题的题解
using System.ComponentModel;

namespace lesson8练习题
{
    //写一个用于数学计算的静态类，该类中提供计算圆 面积 周长 矩形的面积周长 还有绝对值的操作
    public static  class MathTool
    {
        public static float Pi = 3.14f;
        public static  float mianji(float x)
        {
            return Pi * x * x;
        }
        public static float zhouchang(float x)
        {
            return Pi * x * 2;
        }
        public static int juxingzhouchang(int x,int y)
        {
            return (x + y) * 2;
        }
        public static int juxingmianji(int x,int y)
        {
            return x* y;
        }
        public static int jueduizhi(int x)
        {
            if(x>0)
            {
                return x;
            }
            else
            {
                return -x;
            }
        }
    }
    internal class Program
    {
        static void Main(string[] args)
        {

            Console.WriteLine("圆的面积是：{0}",MathTool.mianji(3));
            Console.WriteLine("圆的周长是：{0}",MathTool.zhouchang(3));
            Console.WriteLine("矩形的周长是：{0}",MathTool.juxingzhouchang(3,4));
            Console.WriteLine("矩形的面积是：{0}",MathTool.juxingmianji(3,4));
            Console.WriteLine("您输入数字的绝对值是：{0}", MathTool.jueduizhi(-7));
            Console.WriteLine("您输入数字的绝对值是：{0}", MathTool.jueduizhi(5));
        }
    }
}
