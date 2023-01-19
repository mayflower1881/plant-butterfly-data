# plant-butterfly-data

Analysis code for bipartite graph

bmat=as.matrix(read.csv(file = "/home/tejaswini/Desktop/Butterflyplantdata.csv" , sep = "\t", header=T, row.names=1))

bmat

library(igraph)
bg=graph_from_incidence_matrix(bmat)
bg

V(bg)$type #Display the vertex types. They are "FALSE" or "TRUE"

library(bipartite)
plotweb(bmat) #the base function for bipartite network plot
