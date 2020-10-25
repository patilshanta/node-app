import requests


url = 'https://mirrors.estointernet.in/apache/tomcat/tomcat-9/v9.0.39/bin/apache-tomcat-9.0.39-windows-x64.zip'
r = requests.get(url, allow_redirects=True)

open('tomcat.zip', 'wb').write(r.content)
