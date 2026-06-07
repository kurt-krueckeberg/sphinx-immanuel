# sphinx-immanuel setup

## Set up

```{code-text}
mkdir sphinx-immanuel
cd sphinx-immanuel
cp ~/gens/requirements.txt .
cp ~/gens/.gitignore .
python3 -m venv .venv
source .venv/bin/activate
pip install pip --upgrade
pip install -r requirements.txt
cp ~/gens/_toc.yml .
cp ~/gens/_config.yml
cp -r ~/gens/_static .
```

## Alter `_config.yml`

Change:
- `title:`
- `url:`
- If needed, adjust `intersphinx_mapping:` from something like

  ```{code-text}
  sphinx:
    config:
      external_toc_exclude_missing: true
      intersphinx_mapping: 
        nla:
          - "https://nla.krueckeberg.org/"
          - "https://nla.krueckeberg.org/objects.inv"
  ```
  to be whatever you need.


## Alter `_toc.yml`

