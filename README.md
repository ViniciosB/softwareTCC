# softwareTCC
source venv/bin/activate
cat requirements.txt | xargs -n 1 pip install
sed -i 's/==/>=/g' requirements.txt
pip install -r requirements.txt --upgrade

