SHELL := /bin/bash

config.env:
	echo "PROM_HOST=$(shell op read "op://Lab/Grafana Cloud Metrics/website")" > config.env
	echo "PROM_USERNAME=$(shell op read "op://Lab/Grafana Cloud Metrics/username")" >> config.env
	echo "PROM_PASSWORD=$(shell op read "op://Lab/Grafana Cloud Metrics/password")" >> config.env
