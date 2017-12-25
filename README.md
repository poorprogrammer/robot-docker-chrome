docker build -t docker-robot-framework .


docker run --rm \
-e ROBOT_TESTS=/robots/ \
-e BROWSER=firefox \
-v $(pwd)/robots:/robots \
-ti docker-robot-framework
