prepare-chart:
	CHART_FILES="Chart.yaml"; \
	for chart in $$CHART_FILES; do \
		yq eval -i '.version = "${VERSION}"' $$chart; \
		yq eval -i '.appVersion = "${VERSION}"' $$chart; \


release: prepare-chart
release-dev: prepare-chart
