
using ConsoleApp1;

start:


Practicheskaya2 pract2 = new Practicheskaya2();

string simb;

Console.WriteLine("ввести первое число");
double x = Convert.ToDouble(Console.ReadLine());


Console.WriteLine("ввести действие");
simb = Convert.ToString(Console.ReadLine());

Console.WriteLine("ввести второе число");
double y = Convert.ToDouble(Console.ReadLine());



switch (simb)
{
	case "+":
		pract2.plus(x, y);
		goto start;
	case "-":
		pract2.minus(x, y);
		goto start;
	case "*":
			pract2.umnoshenie(x, y);
		goto start;
	case "/":
			pract2.delenie(x, y);
		goto start;
	case "степень":
		pract2.stepen(x, y);
		goto start;
	case "sqrt":
		pract2.sqrt(x, y);
		goto start;
	case "округление":
		pract2.okryglenie(x, y);
		goto start;
	case "арксинус":
		pract2.arksin(x, y);
		goto start;
	case "площадь прямоугольника":
		pract2.ploshadpr(x, y);
		goto start;
	case "тангенс":
		pract2.tan(x, y);
		goto start;
	case "гиперболический тангенс":
		pract2.tanh(x, y);
		goto start;
	case "периметр прямоугольника":
		pract2.perimetr(x, y);
		goto start;
	case "площадь куба":
		pract2.plcube(x);
		goto start;
	default:
        Console.WriteLine("Вы не ввели действие");
        Console.WriteLine("ошибка");
		break;
}
