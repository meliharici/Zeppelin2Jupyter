## Zeppelin2Jupter: A conversion tool for Jupyter and Zeppelin notebooks

**Author**: Mehmet Melih Arıcı. <br>
For any questions: mehmet.melih.arici@gmail.com

### Requirements

- Python 3.6 or higher

### Zeppelin to Jupyter

If you want to convert your Zeppelin notebook to a Jupyter notebook, download your Zeppelin notebook as a .json file. Then, run the following command to generate Jupyter .ipynb file.

`python convert.py --method z2j --file_path JSON_FILE_PATH`

### Jupyter to Zeppelin

If you want to convert your Jupyter notebook to a Zeppelin notebook, download your Jupyter notebook as a .ipynb file. Then, run the following command to generate Zeppelin .json file.

`python convert.py --method j2z --file_path IPYNB_FILE_PATH`

If you also want to add the identifier of your interpreter, you can add %interpreter_name on top of each cell. For instance, if the name of your interpreter is **python3_7.ipython**, the tool can add **%python3_7.ipython** on top of each cell. This is optional but if you want to add, run the previous command with a minor modification:

`python convert.py --method j2z --file_path IPYNB_FILE_PATH --interpreter INTERPRETER_NAME`