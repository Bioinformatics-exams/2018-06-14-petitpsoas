# UE génétique médicale examen 2018-06-14
Salerno Chloé
https://frama.link/chloesalerno2018
## Exercice 1
### Q1
Les gènes CDKL5, MEPC2 et FOXG1 sont impliqués dans le syndrome de Rett.
### Q2
Les variants se trouvent dans le gène CDKL5 (Mutalyser).
### Q3
Le gène se trouve sur le chromosome X.
### Q4
La transmission est dominante liée à l'X.
### Q5
La maladie s'exprime chez les porteurs hétérozygotes d'un allèle déficient. En effet c'est une maladie dominante.
### Q6
Un homme atteint ne peut pas transmettre la maladie à son fils, car il ne lui transmet que le chromosome Y. En revanche, il transmet la maladie à toutes ses filles, qui seront toutes malades. Une femme malade peut transmettre la maladie à ses filles et ses garçons.
### Q7
* On note variant 1 (NM_003159.2:c.2593C>T) et variant 2 (NM_003159.2:c.2995G>A).
* La notation protéique pour le variant 1 est: NM_003159.2(CDKL5_i001):p.(Gln865*)
* La notation protéique du variant 2 est: NM_003159.2(CDKL5_i001):p.(Val999Met)
### Q8
* NM: signifie qu'il s'agit d'un transcrit (ARNm)
* 003159 et 003159: numéro des transcrits 1 et 2 respectivement
* .2: version des transcrits
* CDKL5: nom du gène
* i001: isoforme 
* p: notation protéique
* (Gln865*): une glutamine en position 865 est remplacée par un codon stop (mutation non-sens)
* (Val999Met): une Valine est remplacé par une methionine en position 999 de la protéine (mutation faux-sens)
### Q9
* Pour le variant 1, la variation est non-sens (elle entraine l'apparition d'un codon stop).
* Pour le variant 2, la variation est faux-sens (remplacement d'une valine par une methionine).
### Q10
* Pour le variant 1, on trouve dans la base de données que le variant est pathogène: http://mecp2.chw.edu.au/cdkl5/cdkl5_variant_results_copy.php?display%5B%5D=cdna&display%5B%5D=prot&display%5B%5D=type&display%5B%5D=path&display%5B%5D=cit&display%5B%5D=snp&mutation=sys_name&m_field=c.2593C%3ET&reference=authors&r_field=&mut_domain=&id=&timing=last_updated&time_int=
* Pour le variant 2, on trouve que c'est un variant bégnin: http://mecp2.chw.edu.au/cdkl5/cdkl5_variant_results_copy.php?display%5B%5D=cdna&display%5B%5D=prot&display%5B%5D=type&display%5B%5D=path&display%5B%5D=cit&display%5B%5D=snp&mutation=sys_name&m_field=c.2995G%3EA&reference=authors&r_field=&mut_domain=&id=&timing=last_updated&time_int=
* Je pense donc d'après cette base de données que le variant 1 est responsable de la maladie. Il est d'ailleurs décrit dans la littérature: https://www.ncbi.nlm.nih.gov/pubmed/?term=23583054
### Q11
La notation HGVS est NC_000023.10:g.18646587C>T
### Q12
* NC signifie *complete genomic molecule* c'est à dire que l'on se base sur la molécule d'ADN
* 000023: chromosome 23
*.10: version 10 du chromosome
* g: notation génomique
* 18646587C>T: en position 18646587 changement de base C (référence) en T (variation).
### Q13
* Variant 1: non trouvé dans GnomAD: http://gnomad.broadinstitute.org/variant/X-18646587-C-T
* Variant 2: conversion en HGVS grace à Mutalyser (NC_000023.10:g.18671566G>A) puis recherche dans GnomAD, on le trouve dans cette base de données: http://gnomad.broadinstitute.org/variant/X-18671566-G-A
### Q14
Le variant 1 n'est pas trouvé, le variant 2 a une fréquence de 0.01055 (relativement fréquent dans la population générale).
## Exercice 2
### Q1
* a) Après avoir effectué le séquençage du génome, et filtré les variants selon certains critères, on a regardé si les variants restants étaient déjà décrits comme pathogènes dans la littérature (base de données OMIM *Online Mendelian Inheritance in Man*).
* b) Les auteurs ont également vérifié si les variants étaient décrits dans une autre base de données DDGP2 (*Developmental Disorders Genotype-to-Phenotype database*) et dans un article de la littérature publié par Kochinke.
### Q2
Les variants sont échelonnés en 5 grades, du plus pathogène au moins délétère:
* Certainement pathogène (avec une probabilité de >0.99 d'être pathogène)
* Probablement pathogène (probabilité comprise entre 0.95 et 0.99)
* Incertain (probabilité entre 0.05 et 0.949)
* Probablement pas pathogène ou avec un retentissement clinique faible (probabilité entre 0.001 et 0.049)
* Non pathogène ou sans retentissement clinique (probabilité <0.001)
Il existe d'autres classification de variants, notamment celle de l'ACMG Guidelines (DOI de l'article: 10.1038/gim.2015.30).
### Q3
* a) La notation HGVS (NM_001190274.1) est le numéro d'accession du transcrit dans la base de données (RefSeq). NM signifie que l'on fait référence à un transcrit (ARNm), suivi de son numéro d'accession qui lui est unique, puis de son numéro de version.
* b) HGVS signifie *Human genome variation society*, elle a recommandé des notations particulières pour classifier les variants.
* c) GRCh37/h19 est le génome de référence utilisé par cette étude pour réaliser l'alignement des séquences lors du séquençage du génome. La dernière version est GRCh38 mais en pratique nous utilisons encore très souvent la même version que dans l'étude.
### Q4
* Pour l'individu 1, les auteurs ont d'abord séquencé l'exome, puis grace à un échantilon sanguin de l'individu 1, de la mère et du père, ils ont complété l'analyse avec la technique *SureSelect XT Human 
All Exon 50 Mb v5 kits* et un séquençage haut débit Illumina. On a ensuite réalisé l'alignement des séquences grace au logiciel BWA. Puis la filtration des variants avec  *varFilter script*.
* Pour l'individu 2, ils ont procédé de même.
### Q5
Les méthodes de séquençage nouvelle génération comme Illumina utilisé dans l'article ont l'avantage d'être moins couteuses et offrent un aperçu du génome entier. Cependant, les erreurs sont plus fréquentes qu'avec le *Gold Standard* qui est le séquençage de Sanger. On réalise donc d'abord un séquençage haut débt, puis on confirme grâce à un séquençage de Sanger la partie du gène concerné uniquement (chez l'individu et chez ses parents). On confirme ainsi la variation de novo, si la mutation est présente uniquement chez l'enfant et pas chez ses parents.
### Q6 
* Le patient 1 est porteur d'une variation hétérozygote délétère de novo (une insertion). Elle est localisé juste en aval de l'exon 3 du gène *FBXO11* et entraîne une altération du site d'épissage.
* Pour le patient 2, la variation conduit à l'apparition d'un codon stop, et c'est le seul variant de novo détecté qui a été sélectionné après les différentes méthodes de filtrages appliqués.
### Q7
* Les variations délétères ont été observées de novo pour les 2 individus
* un troisième individu porteur de la même varation que l'individu 2 a été décrit dans la littérature: Martínez et al. 2017)
* 8 autres individus ont été décrits dans la littérature et porteurs d'une mutation sur *FBXO11*, associé à une déficience intellectuelle (Lelieveld et al. 2016)

