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

update: people said the writing in the videos looks ai generated so i asked fable about it. it rewrote part of the conversion script to do a slower pass on fine detail. i ran it on file 003 overnight since its the shortest one. it didnt get to the render step but it wrote this middle step file out, fable says its the recovered surface data: 003_state.bin. i dont know how to read it. ill keep running it.
