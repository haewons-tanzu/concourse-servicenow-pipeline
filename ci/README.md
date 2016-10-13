Upload the Pipeline:

```
fly -t concourse set-pipeline \
	-p spring-music-servicenow \
	-c ci/pipelines/spring.music.yml \
	-l ci/pipelines/credentials.yml

fly -t concourse unpause-pipeline -p spring-music-servicenow
```


Test individual tasks:

```fly -t concourse execute -c \
  ./ci/tasks/build.springmusic.yml \
  --input spring-music=../spring-music```
