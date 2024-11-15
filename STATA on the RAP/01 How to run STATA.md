#How to run STATA on Biobank RAP


Information for this can be found under the [DNA NEXUS documentation webpage](https://documentation.dnanexus.com/user/jupyter-notebooks/stata-in-dxjupyterlab)

To run Stata on the UK Biobank Research Analysis Platform, you can follow these steps:

1. Ensure you have a valid Stata license and have uploaded your license details to the project. The format of this should be

  
```
{
  "license": {
    "serialNumber": "123456789012",
    "code": "aaaa bbbb cccc dddd eeee ffff gggg hhhh iiii",
    "authorization": "xxxx",
    "user": "John Snow",
    "organization": "My Company"
  }
}
```
   
   I uploaded this as .json file onto the project under the upload button. (Written with Windows notepad, saved as.json)
   
Launch the DXJupyterLab app within your UK Biobank project:
a) Open your project
b) Click "Start Analysis"
c) Select "DXJupyterLab with Python, R, Stata, ML"
d) Add your Stata license file as an input
e) Select "Stata" from the Features dropdown
f) Click "Start Analysis"

When you click Monitor in the RAP Toolbar it can be seen once the Jupyter Lab has switched from "waiting" to running and there is a worker URL that can be clicked to open the JupyterLab. NOTE: when clicked shortly after it has switched to running the error message 502 Bad Gateway comes up. It often needs 5 more minutres to launch and then the URL can be clicked without issues and the Jupyter notebook opens
