# Azure Flask Demo

A vanilla Flask app for Azure WebApp publishing.

It follows Azure recommendation setup using Extension and `web.config` FastCGI setup.

Currently this demo works best with **Python 3.5.1** and does not work with `3.5.2`. [see discussion](https://github.com/Microsoft/PTVS/issues/1791)

# Installation Steps

1. Fork this repository to your account
1. Create a WebApp. Basic tier recommended.
1. In WebApp, turn on **Diagnostics Logs** if you want 
1. Click **Extensions** and add `Python 3.5.1 (x86)` extension.
1. If you want to use `3.5.1 x64`, switch to 64bit in **Application Settings**.
1. Setup **Deployment** to forked GitHub repo `master` branch.
1. Click **Advanced Tools** menu.
1. In top menu, click **Debug Console** > **CMD**
1. Type `d:\home\python35\python.exe -m pip install --upgrade -r d:\home\site\wwwroot\requirements.txt`
1. In WebApp, open url in **Overview**.

# Reference
- Azure WebApp+Python recommendation: https://blogs.msdn.microsoft.com/pythonengineering/2016/08/04/upgrading-python-on-azure-app-service/

