import random

def write_in_file(N,m,file):
    with open(file, 'w+') as f:
        for i in range(N):
            strk = ''
            for j in range(m):
                strk += str(random.uniform(-1, 1)) + ','
            f.write(strk[:-1] + '\n' )
def vvod():
    N,m = 0,0
    check = False
    while not check:
        try:
            N = int(input('Введите N (500 < N ≤ 1000) = '))
            m = int(input('Введите m ( 10 < m ≤ 50 ) = '))
            if (N > 500 and N <= 1000 and m > 10 and m <= 50):
                check = True
            else:
                print('Введите значение в диапазоне')
        except:
            print('Введите корректные значения')
    print('Параметрами выбраны N = {0} m = {1}'.format(N,m))
    return N,m

def main():
        v = input('Вы хотите вписать значения самостоятельно? (Y/N) \n')
        if v.upper() == 'Y':
            N,m = vvod()
        else:
            N = random.randint(500,1000)
            m = random.randint(10,50)
            print('Параметрами выбраны рандомные числа N = {0} m = {1}'.format(N,m))
        file = 'vectors.csv'
        write_in_file(N,m,file)
    
    
    
if __name__ == "__main__":
    main()
