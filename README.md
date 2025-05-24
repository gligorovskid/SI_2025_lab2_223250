# SI_2025_lab2_223250

Душан Глигоровски - 223250

2. ![Control Flow Graph](CFGlab2.drawio)


3. Цикломатската комплексност на дадениот код е 9. Добиена е според графот каде што има 25 ребра(Е) и 18 темиња(N). Па според формулата C = E - N + 2, C = 25 - 18 + 2 = 9. 

4. За да се покријат сите statements од функцијата checkCart, потребни се следниве 5 тест случаи: 
1. allItems = null, checkCart(null, "123"), Фрла RuntimeException("allItems list can't be null!")
2. Item без име, checkCart([new Item(null, 1, 100, 0)], "1234567891234567"), Фрла RuntimeException("Invalid item!")
3. Item со цена > 300 и без попуст, checkCart([new Item("exp", 1, 350, 0)], "1234567891234567"), sum = 320 (350 – 30 казна)
4. Невалидна картичка (невалидна должина), checkCart([], "123"),Фрла RuntimeException("Invalid card number!")
5. Празна листа и валидна картичка, checkCart([], "1234567891234567"), sum = 0 (валидно, но празно)

5. За овој критериум ни требаат 4 случаи бидејќи треба да ги опфатиме само ТXX, XTX, XXT, FFF.
if (item.getPrice() > 300 || item.getDiscount() > 0 || item.getQuantity() > 10).
TXX item=Item(320,0,0)
XTX item=Item(320,10,0)
XXT item=Item(320,0,120)
FFF item=Item(220,-10,-10)






