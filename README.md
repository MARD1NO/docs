### Usage

1. pip3 install -r requirements.txt

2. apt-get install doxygen

3. change your path:

```
/FluidDoc 改成你 clone下来的docs仓库路径，如 /home/paddle/docs
```

4. generate en docs
```
cd /home/paddle/docs/docs/api
python gen_doc.py
```

5. generate en html
```
cd /home/paddle/docs
sphinx-build -b html -j 12 -d /var/doctrees -c /home/paddle/docs/ci_scripts/doc-build-config/en /home/paddle/docs/docs  /home/paddle/docs/output/en/develop
```

6. generate cn html 
```
sphinx-build -b html -j 12 -d /var/doctrees -c /home/paddle/docs/ci_scripts/doc-build-config/zh /home/paddle/docs/docs  /home/paddle/docs/output/zh/develop
```
