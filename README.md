# OPENCV_Python3.9
git clone https://github.com/iandow/opencv_aws_lambda

cd OPENCV_Python3.9

docker build --tag=lambda-layer-factory:latest .

docker run --rm -it -v $(pwd):/data lambda-layer-factory cp /packages/cv2-python39.zip /data
