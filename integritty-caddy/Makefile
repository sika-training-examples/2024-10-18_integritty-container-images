default: build-and-push

cert:
	lego --email ondrejsika@ondrejsika.com --dns cloudflare \
		--domains local.sikademo.com \
		--domains '*.local.sikademo.com' \
		run

build-and-push:
	docker build -t ttl.sh/integritty/integritty-caddy .
	docker push ttl.sh/integritty/integritty-caddy
