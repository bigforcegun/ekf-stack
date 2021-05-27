# Elastic Kibana Filebeat fast stack

Source - https://github.com/gnokoheat/elk-with-filebeat-by-docker-compose

## Work flow

- logs -> filebeat -> elasticsearch <- kibana

## Usage

1. Clone Repo
2. Change logs dir in docker-compose file to app logs dir (or make link)
3. Run

```bash
docker-compose up 
```

4. Go to kibana http://localhost:5601/app/management/kibana/indexPatterns

5. Add `app-logs-*` index pattern

6. Explore your logs!

## Issues

If something went wrong - clear all setup with

```bash
docker-compose down
docker-compose rm -v
```


