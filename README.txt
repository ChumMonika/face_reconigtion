To run
1. Create env: python -m venv venv
	then activate: venv\Scripts\activate

2. Install libraries (skip if already installed)
	pip install -r requirements.txt
	pip install ipykernel
	python -m pip install --upgrade pip
	python -m pip install tensorflow

3. Download model file:
	https://drive.google.com/file/d/1uiOev0Dsxpz1va-8nXZRrxG4JUWNst_B/view?usp=sharing
	Put into: face_demo/model/

Test mode (single image or quick webcam test)
- Use training/arcface_train.ipynb
- Run all cells in order
- For webcam, press q to exit

Deployment mode (attendance system)
- Use deployment/recognition_fixed.ipynb
- Run cells in order:
  - Setup + helpers
  - Register users (manual files or scanning)
  - Live attendance monitor
- Press q to stop webcam

Notes
- Update MODEL_PATH and CLASS_PATH in the notebook if your file names or folders are different.