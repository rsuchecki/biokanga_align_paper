# Introduction

* Expand on bread wheat genome challanges
    * polyploid
    * repeats

## Existing aligners

how detailed do we need to be?
different alignment approaches. cover pseudo alignment? ie kallisto, salmon? 


# Methods

* Reference genome/s (probably one is enough? can we quantify 'complexity'? ie repeats/duplications/syntenic regions with limited polymorphisms... ideally from existing work)
    * Salzburg
    * Clavijo
    * one would be enough, but in a pipeline there should be none or very little overhead of having 2
* Align: (what parameter space? can't be too complete)
    * DNA reads (bioplatforms?)
    * simulated reads
      * can we use biokanga simreads?
      * and/or some third-party?
* Measure:
    * Standard parameters (time/cores blah blah)
    * %aligned in different classes (unaligned, unique etc)
    * Accuracy for simulated reads
    * SNP calling? Typically this is done with a different tool to the aligner - are we introducing SNP calling as well? unsure. could work well with bioplatforms data.

# Results

## Simulated reads

I can imagine a figure showing the fate of reads under different aligners. A sort of sankey diagram showing where they end up, and whether it's the best place or not. 

## bioplatforms reads

Summary of different SNPs reported (ie what is the overlap in the SNPs identified using the different aligners - would need to use the same SNPs caller on the BAM output I guess)? I don't actually know what the differences would look like. Would be nice to have an example or two of where a difference is. Maybe this is really down to parameters (ie how many reads you need to trust the call?)
