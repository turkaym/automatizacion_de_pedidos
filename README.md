# ESTRUCTURA DEL PROGRAMA

pedido_automatizado/
├── capture.py                     # endpoint para subir/guardar la imagen del pedido.
├── preprocess.py                  #  funciones de OpenCV para limpiar la imagen. 
├── ocr_service.py                 # ocr_service.py: invoca Tesseract y devuelve texto.
├── parser.py                      # parser.py: extrae líneas “cantidad + unidad + producto” y normaliza. 
├── alegra_client.py               # alegra_client.py: cliente para la API de Alegra (stock, facturas).
├── catalog.db                     # catalog.db: SQLite con tu catálogo y sinónimos. 
├── requirements.txt
├── README.md
├── .gitignore
└── validation_ui/                 # validation_ui/: interfaz para revisar y corregir antes de enviar. 
    ├── templates/
    │   └── review.html
    └── static/
        ├── css/
        │   └── style.css
        └── js/
            └── review.js
