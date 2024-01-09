# cmdm-llm-env

## Get started
Please check or modify the ports first
```
ports:
  - 48888:8888  # make sure port 48888 is not used; or change it
```
Then,
```
$ docker-compose up --build -d
$ docker exec -it llm-dev bash
```

### Create a jupyter notebook
```
# in container
$ nohup jupyter notebook --ip=0.0.0.0 --port=8888 --allow-root --NotebookApp.token=PASSWORD &
```
Then, you can access jupyter notebook at port 48888 (dependent on your modification) with your password `PASSWORD`