for i in G.nodes():
    nodes_list.append(i)
    f1 = 0 
    f2 = 0
    k4 = 0
    d = 0
    I = 0
    F = 0
    neiks1 = 0
    j = G.neighbors(i)
    for j1 in j:
        neiks1 = neiks1 + c[j1]
    for s in combined_neighbors[i]:
        if not s == i: 
            f1 = dx[i]*math.log(degree_sums[i] + 1, 2)
            f2 = dx[s]*math.log(degree_sums[s] + 1, 2)
            k4 = (neiks1)**2
            d = df.loc[i, s]
            F = k4*f1*(2*average_clustering*f2+1)/d**2
            I = I + F
    list1.append(I)
dic = dict(zip(nodes_list, list1))
