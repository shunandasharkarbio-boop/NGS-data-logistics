Collapse data into a single dataset
-------------------------
We now extracted meaningful fields from VCF datasets. But they still exist as a collection. To move towards secondary analysis we need to collapse this collection into a single dataset. “Collapsing” simply concatenates the content of collection elements and attaches sample IDs, so that we know which line in the concatenated file corresponds to which sample:
<p align="center">
  <img src="./Collapse.svg" alt="Collapse.svg" width="100%">
</p>
