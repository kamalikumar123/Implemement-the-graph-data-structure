# Implemement-the-graph-data-structure
class Graph {
  class Edge {
    int src, dest;
  }
  int vertices, edges;
  Edge[] edge;
  Graph(int vertices, int edges) {
    this.vertices = vertices;
    this.edges = edges;
    edge = new Edge[edges];
    for(int i = 0; i < edges; i++) {
      edge[i] = new Edge();
    }
  }
public static void main(String[] args) {
    int noEdges = 8;
    Graph g = new Graph(noVertices, noEdges);

    
    g.edge[0].src = 1;   
    g.edge[0].dest = 2;

    g.edge[1].src = 1;   
    g.edge[1].dest = 3;

    g.edge[2].src = 1;  
    g.edge[2].dest = 4;

    g.edge[3].src = 2;  
    g.edge[3].dest = 4;

    g.edge[4].src = 2;  
    g.edge[4].dest = 5;

    g.edge[5].src = 3;   
    g.edge[5].dest = 4;

    g.edge[6].src = 3;   
    g.edge[6].dest = 5;

    g.edge[7].src = 4;  
    g.edge[7].dest = 5;
    for(int i = 0; i < noEdges; i++) {
      System.out.println(g.edge[i].src + " - " + g.edge[i].dest);
    }

  }
}
