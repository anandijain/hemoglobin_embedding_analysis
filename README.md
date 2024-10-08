# review of protein models 

* pre stream get keys set up in env so not leaked 
* hemaglobin mutated and not mutated for both ESM and the proprietary * ginkgo model 
* see how they're different? 
* ESMTOkenizer docs nowhere to be found ...
* what is a transform and how is it different to the embedding api 
* https://www.uniprot.org/uniprotkb/P68871/entry normal hbb
* https://rest.uniprot.org/uniprotkb/P68871.fasta normal hbb fasta 
* hbs mutation https://web.expasy.org/variant_pages/VAR_002863.html 
* https://www.uniprot.org/diseases/DI-02306
* also do alphafold server on hbb and hbs 
* do alphafold 3 with the entire complex (normal and mutated )
* https://chatgpt.com/share/66ec9d75-7ce8-8009-bc55-bff381d8e327
* do overview of 1) basic mendelian genetics and how incredible hetrozygous advantage is 


ESM2 paper https://www.biorxiv.org/content/10.1101/2022.07.20.500902v1 


normal hbb
MVHLTPEEKSAVTALWGKVNVDEVGGEALGRLLVVYPWTQRFFESFGDLSTPDAVMGNPKVKAHGKKVLGAFSDGLAHLDNLKGTFATLSELHCDKLHVDPENFRLLGNVLVCVLAHHFGKEFTPPVQAAYQKVVAGVANALAHKYH

HbS 
MVHLTPVEKSAVTALWGKVNVDEVGGEALGRLLVVYPWTQRFFESFGDLSTPDAVMGNPKVKAHGKKVLGAFSDGLAHLDNLKGTFATLSELHCDKLHVDPENFRLLGNVLVCVLAHHFGKEFTPPVQAAYQKVVAGVANALAHKYH


normal hba 
MVLSPADKTNVKAAWGKVGAHAGEYGAEALERMFLSFPTTKTYFPHFDLSHGSAQVKGHGKKVADALTNAVAHVDDMPNALSALSDLHAHKLRVDPVNFKLLSHCLLVTLAAHLPAEFTPAVHASLDKFLASVSTVLTSKYR

what we're feeding to alphafold: 
https://www.rcsb.org/structure/1gzx 
or the deoxy version 
https://www.rcsb.org/structure/1a3n


From wikipedia https://en.wikipedia.org/wiki/Sickle_cell_disease#Genetics

This is normally a benign mutation, causing no apparent effects on the secondary, tertiary, or quaternary structures of haemoglobin in conditions of normal oxygen concentration. However, under low oxygen concentration, HbS polymerizes and forms fibrous precipitates because the deoxy form of haemoglobin exposes a hydrophobic patch on the protein between the E and F helices (Phe 85, Leu 88).[70]


## ginkgo api review 
links:
* technical review https://www.ginkgobioworks.com/2024/09/17/aa-0-protein-llm-technical-review/ 
* announcement https://www.ginkgobioworks.com/2024/09/17/ginkgo-model-api-ai-research/
* docs https://omni-3.gitbook.io/ginkgo
* playground https://models.ginkgobioworks.ai/playground


pros: 
* pretty nice playground
* easy api (none of that google project + oauth nonsense)


cons: 
* very limited models just embedding and fill mask - not the most useful - no structure prediction also * small only 650 M whereas the ESM2 paper trains up to 15B
* only let me get in with my edu email 
* charged me (used my trial requests) on requests that errored (at parse time)
* no way to cycle api keys (wtf )
* docs are a 4/10 - specifically "Please refer to the ESMTokenizer docs for more information on the inputs."
* no public issue tracker or feedback button just a help email
* would like to see a demo video or intro into a practical and useful use case 

overall a 5/10 experience. happy to see its not impossible to at least use, despite how limited it is.
