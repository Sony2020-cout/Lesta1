#include <iostream>



void main()
{
    setlocale(LC_CTYPE, ".1251");
    int h, a, w;
    std::cout << "Введите высоту \nh = ";
    std::cin >> h;
    std::cout << "Введите ширину \nw = ";
    std::cin >> w;
    std::cout << "Введите величину ячейки .\na = ";
    std::cin >> a;
    for (int i = 0; i < h; i++)
    {
        for (int jj = 0; jj < a; jj++)
        {
            for (int j = 0; j < w; j++)
            {
                for (int ii = 0; ii < a; ii++)
                {
                    ((i + j) % 2) ? (std::cout << '-') : (std::cout << 'x');
                }
            }
            std::cout << '\n';
        }
    }
    std::cout << "\n\n\n";
    system("pause");
}
