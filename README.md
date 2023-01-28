# Networks

The purpose of this project is to learn how to plot networks. More importantly, learning how to deal with large networks which may be problematic for network visualisation. In this project, I will use a data set from the paper 'Local Higher-order Graph Clustering', Yin et al. (2017), which is an anonymised email data set from a large European research institution. The data set contains directed edges in the network when one person sents at least one email to another. Furthermore, the emails only represent communication within the institution. The network plot produced resulted in a plot that was unreadable and one that you could not get any information from, therefore, I condensed the data into a more informative plot using a dendrogram. 

# Findings

After cleaning up the data, the initial plot of the complete network was too condense and there were too many edges and nodes that overlapped with each other, causing the plot to be unreadable. This initial plot is shown below: 

![](https://github.com/kellyngsf/euemail_networks/blob/main/images/euemail_network_initialplot.png)

I then contracted the network so that in the new network, there is a node for each department, one directed edge from one department to another (if an email is sent between them), and finally, each edge will have a weight that is equal to the number of people in one department that send an email to another department. This contracted network is shown below.

![](https://github.com/kellyngsf/euemail_networks/blob/main/images/euemails_network1.png)

As seen on the network, we can see the number labelled nodes and edges that are colored to show their weight, however, because it's such a large network, it's hard to find any relationships or patterns between departments. Hence, I tried to plot the data in a different type a plot, a dendrogram that shows how close relations between departments are. This plot is shown below and we can immediately see a more clean and organized plot that shows which departments have a close relationship to each other through a department hierarchy. 

![](https://github.com/kellyngsf/euemail_networks/blob/main/images/euemail_networks2.png)

### References:
Yin, H., Benson, A. R., Leskovec, J., and Gleich, D. F. (2017). Local higher-order graph clustering. In Proceedings of the 23rd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining, KDD ’17, page 555–564, New York, NY, USA. Association for Computing Machinery.
