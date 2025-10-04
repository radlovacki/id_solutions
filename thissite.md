# Како да креираш овакав веб сајт?

```text
C:\dev\id_solutions>python -m venv venv

C:\dev\id_solutions>venv\Scripts\activate

(venv) C:\dev\id_solutions>

(venv) C:\dev\id_solutions>pip --version
pip 25.1.1 from C:\dev\id_solutions\venv\Lib\site-packages\pip (python 3.13)

(venv) C:\dev\id_solutions>pip install mkdocs-material
Collecting mkdocs-material
  Downloading mkdocs_material-9.6.21-py3-none-any.whl.metadata (19 kB)
Collecting babel~=2.10 (from mkdocs-material)
  Using cached babel-2.17.0-py3-none-any.whl.metadata (2.0 kB)
Collecting backrefs~=5.7.post1 (from mkdocs-material)
  Downloading backrefs-5.9-py313-none-any.whl.metadata (3.2 kB)
Collecting colorama~=0.4 (from mkdocs-material)
  Using cached colorama-0.4.6-py2.py3-none-any.whl.metadata (17 kB)
Collecting jinja2~=3.1 (from mkdocs-material)
  Using cached jinja2-3.1.6-py3-none-any.whl.metadata (2.9 kB)
Collecting markdown~=3.2 (from mkdocs-material)
  Downloading markdown-3.9-py3-none-any.whl.metadata (5.1 kB)
Collecting mkdocs-material-extensions~=1.3 (from mkdocs-material)
  Using cached mkdocs_material_extensions-1.3.1-py3-none-any.whl.metadata (6.9 kB)
Collecting mkdocs~=1.6 (from mkdocs-material)
  Using cached mkdocs-1.6.1-py3-none-any.whl.metadata (6.0 kB)
Collecting paginate~=0.5 (from mkdocs-material)
  Using cached paginate-0.5.7-py2.py3-none-any.whl.metadata (11 kB)
Collecting pygments~=2.16 (from mkdocs-material)
  Using cached pygments-2.19.2-py3-none-any.whl.metadata (2.5 kB)
Collecting pymdown-extensions~=10.2 (from mkdocs-material)
  Downloading pymdown_extensions-10.16.1-py3-none-any.whl.metadata (3.1 kB)
Collecting requests~=2.26 (from mkdocs-material)
  Downloading requests-2.32.5-py3-none-any.whl.metadata (4.9 kB)
Collecting MarkupSafe>=2.0 (from jinja2~=3.1->mkdocs-material)
  Downloading markupsafe-3.0.3-cp313-cp313-win_amd64.whl.metadata (2.8 kB)
Collecting click>=7.0 (from mkdocs~=1.6->mkdocs-material)
  Downloading click-8.3.0-py3-none-any.whl.metadata (2.6 kB)
Collecting ghp-import>=1.0 (from mkdocs~=1.6->mkdocs-material)
  Using cached ghp_import-2.1.0-py3-none-any.whl.metadata (7.2 kB)
Collecting mergedeep>=1.3.4 (from mkdocs~=1.6->mkdocs-material)
  Using cached mergedeep-1.3.4-py3-none-any.whl.metadata (4.3 kB)
Collecting mkdocs-get-deps>=0.2.0 (from mkdocs~=1.6->mkdocs-material)
  Using cached mkdocs_get_deps-0.2.0-py3-none-any.whl.metadata (4.0 kB)
Collecting packaging>=20.5 (from mkdocs~=1.6->mkdocs-material)
  Using cached packaging-25.0-py3-none-any.whl.metadata (3.3 kB)
Collecting pathspec>=0.11.1 (from mkdocs~=1.6->mkdocs-material)
  Using cached pathspec-0.12.1-py3-none-any.whl.metadata (21 kB)
Collecting pyyaml-env-tag>=0.1 (from mkdocs~=1.6->mkdocs-material)
  Using cached pyyaml_env_tag-1.1-py3-none-any.whl.metadata (5.5 kB)
Collecting pyyaml>=5.1 (from mkdocs~=1.6->mkdocs-material)
  Downloading pyyaml-6.0.3-cp313-cp313-win_amd64.whl.metadata (2.4 kB)
Collecting watchdog>=2.0 (from mkdocs~=1.6->mkdocs-material)
  Using cached watchdog-6.0.0-py3-none-win_amd64.whl.metadata (44 kB)
Collecting charset_normalizer<4,>=2 (from requests~=2.26->mkdocs-material)
  Downloading charset_normalizer-3.4.3-cp313-cp313-win_amd64.whl.metadata (37 kB)
Collecting idna<4,>=2.5 (from requests~=2.26->mkdocs-material)
  Using cached idna-3.10-py3-none-any.whl.metadata (10 kB)
Collecting urllib3<3,>=1.21.1 (from requests~=2.26->mkdocs-material)
  Using cached urllib3-2.5.0-py3-none-any.whl.metadata (6.5 kB)
Collecting certifi>=2017.4.17 (from requests~=2.26->mkdocs-material)
  Using cached certifi-2025.8.3-py3-none-any.whl.metadata (2.4 kB)
Collecting python-dateutil>=2.8.1 (from ghp-import>=1.0->mkdocs~=1.6->mkdocs-material)
  Using cached python_dateutil-2.9.0.post0-py2.py3-none-any.whl.metadata (8.4 kB)
Collecting platformdirs>=2.2.0 (from mkdocs-get-deps>=0.2.0->mkdocs~=1.6->mkdocs-material)
  Downloading platformdirs-4.4.0-py3-none-any.whl.metadata (12 kB)
Collecting six>=1.5 (from python-dateutil>=2.8.1->ghp-import>=1.0->mkdocs~=1.6->mkdocs-material)
  Using cached six-1.17.0-py2.py3-none-any.whl.metadata (1.7 kB)
Downloading mkdocs_material-9.6.21-py3-none-any.whl (9.2 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 9.2/9.2 MB 32.4 MB/s eta 0:00:00
Using cached babel-2.17.0-py3-none-any.whl (10.2 MB)
Downloading backrefs-5.9-py313-none-any.whl (399 kB)
Using cached colorama-0.4.6-py2.py3-none-any.whl (25 kB)
Using cached jinja2-3.1.6-py3-none-any.whl (134 kB)
Downloading markdown-3.9-py3-none-any.whl (107 kB)
Using cached mkdocs-1.6.1-py3-none-any.whl (3.9 MB)
Using cached mkdocs_material_extensions-1.3.1-py3-none-any.whl (8.7 kB)
Using cached paginate-0.5.7-py2.py3-none-any.whl (13 kB)
Using cached pygments-2.19.2-py3-none-any.whl (1.2 MB)
Downloading pymdown_extensions-10.16.1-py3-none-any.whl (266 kB)
Downloading requests-2.32.5-py3-none-any.whl (64 kB)
Downloading charset_normalizer-3.4.3-cp313-cp313-win_amd64.whl (107 kB)
Using cached idna-3.10-py3-none-any.whl (70 kB)
Using cached urllib3-2.5.0-py3-none-any.whl (129 kB)
Using cached certifi-2025.8.3-py3-none-any.whl (161 kB)
Downloading click-8.3.0-py3-none-any.whl (107 kB)
Using cached ghp_import-2.1.0-py3-none-any.whl (11 kB)
Downloading markupsafe-3.0.3-cp313-cp313-win_amd64.whl (15 kB)
Using cached mergedeep-1.3.4-py3-none-any.whl (6.4 kB)
Using cached mkdocs_get_deps-0.2.0-py3-none-any.whl (9.5 kB)
Using cached packaging-25.0-py3-none-any.whl (66 kB)
Using cached pathspec-0.12.1-py3-none-any.whl (31 kB)
Downloading platformdirs-4.4.0-py3-none-any.whl (18 kB)
Using cached python_dateutil-2.9.0.post0-py2.py3-none-any.whl (229 kB)
Downloading pyyaml-6.0.3-cp313-cp313-win_amd64.whl (154 kB)
Using cached pyyaml_env_tag-1.1-py3-none-any.whl (4.7 kB)
Using cached six-1.17.0-py2.py3-none-any.whl (11 kB)
Using cached watchdog-6.0.0-py3-none-win_amd64.whl (79 kB)
Installing collected packages: paginate, watchdog, urllib3, six, pyyaml, pygments, platformdirs, pathspec, packaging, mkdocs-material-extensions, mergedeep, MarkupSafe, markdown, idna, colorama, charset_normalizer, certifi, backrefs, babel, requests, pyyaml-env-tag, python-dateutil, pymdown-extensions, mkdocs-get-deps, jinja2, click, ghp-import, mkdocs, mkdocs-material
Successfully installed MarkupSafe-3.0.3 babel-2.17.0 backrefs-5.9 certifi-2025.8.3 charset_normalizer-3.4.3 click-8.3.0 colorama-0.4.6 ghp-import-2.1.0 idna-3.10 jinja2-3.1.6 markdown-3.9 mergedeep-1.3.4 mkdocs-1.6.1 mkdocs-get-deps-0.2.0 mkdocs-material-9.6.21 mkdocs-material-extensions-1.3.1 packaging-25.0 paginate-0.5.7 pathspec-0.12.1 platformdirs-4.4.0 pygments-2.19.2 pymdown-extensions-10.16.1 python-dateutil-2.9.0.post0 pyyaml-6.0.3 pyyaml-env-tag-1.1 requests-2.32.5 six-1.17.0 urllib3-2.5.0 watchdog-6.0.0

[notice] A new release of pip is available: 25.1.1 -> 25.2
[notice] To update, run: python.exe -m pip install --upgrade pip



(venv) C:\dev\id_solutions>mkdocs new .
INFO    -  Writing config file: .\mkdocs.yml
INFO    -  Writing initial docs: .\docs\index.md




```
