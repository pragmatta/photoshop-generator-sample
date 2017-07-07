# Photoshop Generator Sample
This is a sample Photoshop Generator plugin using photoshop-generator-core node module enabling HTTP access to Photoshop:
- Open documents (list, change active, close)
- Layer metadata (bounds, children, etc.)
- Layer content 

To deploy the sample plugin 
1) Create a folder
2) Install the module 'npm install photoshop-generator-sample'
3) Copy content from node_modules/photoshop-generator-sample to the folder root
4) Copy the folder to $Photoshop/Plug-ins/Generator
5) Start Photoshop and open a document
6) Open browser and visit
   - http://localhost:8083/ for server info
   - http://localhost:8083/documents for a list of open documents
   - http://localhost:8083/layerdata/DOCUMENT_ID for document root metadata
   - http://localhost:8083/layerdata/DOCUMENT_ID/LAYER_ID for layer metadata
   - http://localhost:8083/layercontent/DOCUMENT_ID/LAYER_ID for layer content as a PNG

