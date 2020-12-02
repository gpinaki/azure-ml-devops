Prerequisite
local repo is integrated with github
azure account 

1. Set up virtualenv:

python3 -m venv ~/.azure-ml-devops
source ~/.azure-ml-devops/bin/activate

2. make install

3.  Run locally

export set FLASK_APP=app.py
python3 -m flask run

4. Now deploy the app in azure

az webapp up -n udacity-ml-app

Verify app is running in http://udacity-ml-app.azurewebsites.net

{
  "URL": "http://udacity-ml-app.azurewebsites.net",
  "appserviceplan": "surpriseforpinaki_asp_Linux_centralus_0",
  "location": "centralus",
  "name": "udacity-ml-app",
  "os": "Linux",
  "resourcegroup": "surpriseforpinaki_rg_Linux_centralus",
  "runtime_version": "python|3.7",
  "runtime_version_detected": "-",
  "sku": "PREMIUMV2",
  "src_path": "//Users//pinakiguha//udacity-git-course//azure-ml-devops"
}

