# Robotframework + Browser com Docker

Os testes ficam dentro do repositório `tests`.
A execução dos testes é feita através do comando:
```bash
docker run --rm -v $(pwd)/tests/:/tests --ipc=host --user pwuser marketsquare/robotframework-browser:latest bash -c "robot --outputdir /tests/output /tests/"
```