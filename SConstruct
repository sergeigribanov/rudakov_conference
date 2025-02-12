import os
# PDFLATEXFLAGS='-shell-escape'
env=Environment(PDFLATEX='pdflatex')
env.Replace(BIBTEX='biber')
env.AppendUnique(PDFLATEXFLAGS='-synctex=1')
documents = ['rudakov-etapipi-2025']

for name in documents:
    env.PDF(target = os.path.join(name + '.pdf'),
    source = os.path.join(name + '.tex'))
