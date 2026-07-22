# btcx-files

first 4kb of two of the 613 files my mining software saved in feb 2018, plus full hex dumps of both.

every file starts with the same 16 bytes:

```
F5 A5 05 5A 5F F5 A5 05 5A 5F F5 A5 05 5A 5F 05
```

claude fable 5 says this matches no known file format. if anyone can identify it let me know.

not sharing full files for now, they are big and i am still converting them.

added a script the llm wrote that checks the structure, run it on the samples: python3 parse_btcx.py 20180213_0417.bin

update: fable changed the script a bit, added a scan that looks for structured parts inside the streams. doesnt flag anything on these two samples, i think theyre just too small (its only the first 4kb).

update: changed the conversion script to do a slower pass on fine detail. re ran file 003 since its the shortest and it wrote out a middle step file instead of getting to the render, says its the recovered surface data. its here as 003_state.bin. i cant read it. still converting the rest in order.

update: someone asked for more than the first 4kb so here is the first 8kb of the same two files (20180213_0417_8k.bin, 20180219_2258_8k.bin). the first 4kb is identical to the older samples if you want to diff them. still not uploading full files, theyre 2tb.

update: file 62 is one of the ones that never converted correctly. here is the first 25mb in case anyone can tell me anything.
