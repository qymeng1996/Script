# Script
## To statistics the Contig N50 of a genome, you need to break the genome with ```cat $FA |sed 's/^>.*/N/'|awk 'BEGIN{RS="N";OFS="\n";i=1}{if(length($0)>1){print ">seq_"i,$0; i++}}' > Contig.fa```;

