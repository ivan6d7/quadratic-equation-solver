def solve(a, b, c):
    res = []
    D = b * b - 4 * a * c

    def root(D):
        b = 0
        while b * b < D:
            b += 1
        else:
            return(b)
        
    rtD = root(D)
    MINUS_ONE = -1
    if D > 0:
        xone1 = b * MINUS_ONE + rtD
        xone2 = xone1 / (2 * a)
        res.append(xone2)
        xtwo1 = b * MINUS_ONE - rtD
        xtwo2 = xtwo1 / (2 * a)
        res.append(xtwo2)
    elif D == 0:
        x1 = b * MINUS_ONE 
        x2 = x1 / (2 * a)
        res.append(x2)
    return res

def test():
    # test for 2 roots
    if solve(5, -7, 2) != [1.0, 0.4]:
        return False
    #test for 1 root
    if solve(1, 2, 1) != [-1]:
        return False
    #test for no roots
    if solve(3, 1, 1) != []:
        return False

if test() == False:
    print("Test didn't work")
else:
    print('ax2+bx+c = 0')
    a = int(input('input a: '))
    b = int(input("input b: "))
    c = int(input('input c: '))

    print (solve(a, b, c))
