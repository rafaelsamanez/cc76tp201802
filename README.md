# cc76tp201802
trabajo de complejidad algoritmica 

...code
def LeeMA2MA(filename):
    """
    Funcion lee un archivo que contiene un grafo en formato de matriz de adyacencia
    y retorna una matriz de adyacencia
    """
    file = open(filename)
    i = -1
    for line in file:
        if i == -1:
            n = int(line)
            G = [None for _ in range(n)]
        else:
            G[i] = [int(x) for x in line.split(' ')]
        i +=1
        
    return G
    
    ...
