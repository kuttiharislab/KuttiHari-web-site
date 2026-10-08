# Kutti Hari website

Static source and container deployment files for the Kutti Hari website.

## Current addresses

- Public preview: <https://kuttihari.cityplug.co.uk/>
- Private CityPlug address: <https://kuttihari.local.cityplug.co.uk/>

## Local preview

```bash
python3 -m http.server 8788
```

Open <http://127.0.0.1:8788/>.

## Container deployment

```bash
docker compose up -d --build
```

The current Apollo deployment binds to `10.1.1.253:8788`. Public and private ingress are managed outside this repository.

## Search indexing

The preview intentionally sends `noindex, nofollow`. Remove that release guard only when the final public-domain cutover is approved.
