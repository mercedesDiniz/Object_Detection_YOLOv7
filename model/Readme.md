# Projeto de Detecção e Classificação de Objetos com Yolo


1. Use algum dos modelos de notebooks disponiveis para inicar um novo projeto.
https://github.com/roboflow/notebooks 
> O utilizado aqui foi o [YOLOv7 Object Detection](https://github.com/roboflow/notebooks#:~:text=YOLOv8%20Classification-,YOLOv7%20Object%20Detection,-YOLOv7%20Instance%20Segmentation)

2. Faça o download do repositório YOLOv7 e instale os requisitos
~~~bash
git clone https://github.com/WongKinYiu/yolov7
cd yolov7
pip install -r requirements.txt
~~~
> A versão atual do YOLOv7 não é compatível com pytorch>1.12.1 e numpy>1.20.1, 
até que as alterações apropriadas sejam feitas no repositório principal, usaremos um fork contendo o código corrigido. Você pode acompanhar o progresso [aqui](https://github.com/roboflow/notebooks/issues/27). 

~~~bash
git clone https://github.com/SkalskiP/yolov7.git
cd yolov7
git checkout fix/problems_associated_with_the_latest_versions_of_pytorch_and_numpy
pip install -r requirements.txt
~~~

3. Instale e faça o download de algum Dataset no [Roboflow](https://universe.roboflow.com/)
~~~bash
pip install roboflow
from roboflow import Roboflow
rf = Roboflow(api_key="7kIgVpnvd8c5pAl1n1ad")
~~~