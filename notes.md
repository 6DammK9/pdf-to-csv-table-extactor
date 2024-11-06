```sh
conda create -n pdf-to-csv-cv-env python=3.6
conda activate pdf-to-csv-cv-env

pip install opencv-python==3.4.4.19

pip install -r requirements.txt

pip install tqdm

python pdf-to-csv-cv.py -p test.pdf
```

- Install tesseract-ocr and set PATH

```sh
python pdf-to-csv-cv.py -p "E:/node_workspace/ura-rag-demo/RAG_V4_241030/poc/pdfs/Chapter 4 3. -Spare Parts-05.pdf"
```

- Compare with `tabula-py`, meanwhile try to parse per page (there is too many misaligned tables)

```sh
# WTF is https://docs.github.com/en/rest/markdown?apiVersion=2022-11-28?
cd "E:\node_workspace\ura-rag-demo\ignore\mdtable2csv"
python mdtable2csv.py "E:/node_workspace/ura-rag-demo/RAG_DOC/hkaa_240912/raw_md/Chapter 4 3. -Spare Parts/Chapter 4 3. -Spare Parts.md"
```