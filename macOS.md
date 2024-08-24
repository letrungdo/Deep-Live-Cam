brew install ffmpeg
brew install python-tk@3.10

python3 -m venv venv
source venv/bin/activate

// --------------------------------------------

pip install -r requirements.txt

pip uninstall onnxruntime onnxruntime-silicon
pip install onnxruntime-silicon==1.13.1


python3 run.py --execution-provider coreml
