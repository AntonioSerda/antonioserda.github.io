---
layout: post
title: APPLICATION OF COMPLEX NETWORK THEORY TO THE VULNERABILITY ANALYSIS OF A SATELLITE NETWORK
---
### Author: Serda Mena, Antonio
### Supervisor: Sevillano Bravo, Enrique
### Colaborating institution: ICAI – Universidad Pontificia Comillas

## Introduction
With the development of new systems based on the Internet of Satellites, it has become necessary to have methods capable of dynamically evaluating the connections of a network. This type of constellation is based on communication between satellites in orbit with the aim of covering large distances and dispensing, as far as possible, with wired infrastructure on the ground. By operating in this way, significant savings in raw materials could be achieved, as well as greater coverage of communication networks.

To avoid the saturation of orbits, due to the increase in the amount of space debris, as well as the appearance of the so-called “megaconstellations”, the interconnection between satellites not belonging to the same constellation has been considered. In this way, when several satellites have processing resources available, sporadic connections between them could be generated to transmit information more efficiently.

This new paradigm poses a high level of complexity as connections can occur suddenly. Therefore, the representation of all network elements in time, as well as their information flows, become key elements for the operation of the system. This can be done using the Complex Network Theory.

This Theory is used to represent, in the form of graphs, sets of elements related to each other by means of links that generate non-trivial topological conditions. It has its origin at the beginning of the present century and advances within it are still being developed.

In this Project a hypothetical satellite network has been represented, using the Globalstar constellation for the month of September 2021, where each satellite is considered as a node of the network and the direct visibility between them, as a link. Several programs have been created in MATLAB to determine the most critical satellites during a time interval and the order of elimination that would generate the least efficient network possible. This is used to determine which satellites are the most important at any given time and to be able to take action accordingly for the future. Two different methods are used for this purpose.

The first one is the “multiplex” method, based on the calculation of the metrics of different networks, defined periodically over a time interval, for which their average values are then calculated and decided accordingly.

The second one is the “monoplex”, based on the grouping of the various binary networks of the multiplex method into a single network of weighted links. The weights of each link represent the ratio of connection time between two satellites. Once the monoplex network is available, its metrics are calculated and decided accordingly.

As the metrics of the two methods cannot be directly compared, it is necessary to create other programs to compare the effectiveness between them. The way to evaluate this consists of comparing the number of matches of the lists of satellites eliminated by each method and their order of elimination with a random probability distribution, as well as comparing the metrics of each method with the metrics of the networks recalculated using the lists of eliminated satellites of the analogous methods.

## Methodology
The different objectives of the project emerged as it was being completed, thanks to the agile methodology employed. Both the theory and the technical aspects of the project were continuously re-evaluated.

Initially, the idea of evaluating the average values of the metrics for the entire interval originated, since this was the most intuitive method, that is, multiplex. Through research on similar cases, the concept of “complex multilayer networks” was discovered. Thanks to this, it was considered to represent the total connection time ratio between satellites in the form of weighted links, that is, by means of the monoplex method. This resulted in two different analysis methods that were not necessarily directly comparable.

Finally, the necessary tests were developed to compare the two methods. First, the probability distribution function used to determine whether the coincident satellites removed by both methods followed a random distribution was identified. This was resolved using combinatorics. The random distribution was then compared to an experimental distribution, being it the result of running several analyses iteratively over time. The goodness-of-fit test performed was Pearson’s χ2 test, used to compare discrete distributions. Finally, the efficiency values of the different methods and their recalculated versions were plotted to determine the possible superiority of any of them and the advantages and disadvantages of each.

## Results
After performing all the relevant tests, the following results were obtained, where the efficiency metric is the one that must decrease to the maximum in the network to obtain the best results for each method.

• A higher level of coincidence between the satellites eliminated by both methods when a number of eliminations similar to half of the network totals have been performed. This implies a higher degree of similarity between both methods for these eliminations. For the last eliminations, the matches between the two methods tended to randomness. This indicates a decrease in the efficiency of the methods from that point on.

• A greater decrease in the efficiency of the multiplex method than that of its recalculated version. This implies that it we cannot be assured that the monoplex method gives better results than the multiplex method.

• A similar level of efficiency between the multiplex method and its recalculated version after the first eliminations of satellites, as well as an increase in efficiency in the first eliminations for the recalculated version of the monoplex method, the original being below and decreasing. Although the recalculated version of the multiplex does not give better results, the recalculated version of the monoplex method does not either and also does not reduce the efficiency for these iterations. This implies that it cannot be assured that the multiplex method gives better results for the first few satellite removals from the network.

• A decrease in the efficiency of the recalculated monoplex method, below that of the monoplex, for the central satellite removals. This implies a higher efficiency of the multiplex method over the monoplex when a number of deletions similar to half of the total satellites in the network have been performed.

• A greater variability in the results of the experiments for the last satellite eliminations, explaining why there is a lower number of coincidences between the lists of eliminated satellites according to each method when there are few satellites left to eliminate.

## Conclusions
In this Project several programs, that allow the analysis of satellite networks, as well as their representation in time and space, have been developed in MATLAB. Thanks to these programs, other related studies can be carried out more easily. All the programs have explanations of their operation and the theoretical foundations of each one are detailed in the memory.

Everything shown here is a small part of what is expected to constitute the processes necessary to generate Internet of Satellites networks. The aim is to obtain a more efficient and faster communications network, so it will be necessary to use less raw materials and energy, as well as to generate less space debris in order to continue using the available orbits in a sustainable way.

## Links
For a complete explanation about how the project works go to [Repositorio Comillas](http://hdl.handle.net/11531/59962).

For the necesary codes to make it function go to [my repository](https://github.com/AntonioSerda/APPLICATION-OF-COMPLEX-NETWORK-THEORY-TO-THE-VULNERABILITY-ANALYSIS-OF-A-SATELLITE-NETWORK) on Github.

## Cite as:
A. Serda Mena. (2022). Aplicación de la teoría de redes complejas al análisis de vulnerabilidades de una red de satélites. http://hdl.handle.net/11531/59962
