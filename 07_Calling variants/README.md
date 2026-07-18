Calling variants
---------
Now we are ready to proceed with variant calling. For this purpose we will use a tool called lofreq. One thing to keep in mind in our case is that the samples are from human blood. In humans Plasmodium parasites exist in haploid state (only zygote is diploid and this stage happens in mosquito). lofreq is specifically designed for calling variants in this scenario.

Realign reads
----------
One of the key issues with accurate identification of sequence variants is normalizing indels (insertions and deletions).
