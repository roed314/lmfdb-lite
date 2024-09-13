# lmfdb-lite
dictionary-based python interface to the L-functions and modular forms database (lmdfb.org)

## Install

```
pip3 install -U git+https://github.com/roed314/lmfdb-lite.git#egg=project[pgbinary]
```
or
```
pip3 install -U git+https://github.com/roed314/lmfdb-lite.git#egg=project[pgsource]
```

## Usage

```python
>>> from lmf import db
>>> sorted(set(name.split("_")[0] for name in db.tablenames))
['artin', 'av', 'belyi', 'bmf', 'char', 'cluster', 'data', 'ec', 'fq', 'g2c', 'gps', 'halfmf', 'hecke', 'hgcwa', 'hgm', 'hmf', 'hmsurfaces', 'inv', 'lat', 'lf', 'lfunc', 'maass', 'mf', 'modcurve', 'modlgal', 'modlmf', 'nf', 'noncong', 'pg', 'quaternion', 'shimcurve', 'shimura', 'smf', 'test', 'weil']
```

More documentation coming soon.