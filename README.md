# sw-ourbox-apps-hello-world

`sw-ourbox-apps-hello-world` is a minimal second `sw-ourbox-apps-*`
publisher repo.

Its job is simple: publish one tiny `hello-world` application image so the
catalog side can prove that an OurBox application catalog may consume images
from more than one apps repository.

## Published application

- `hello-world`
  - static hello-world page served from nginx
  - image: `ghcr.io/techofourown/sw-ourbox-apps-hello-world/hello-world`

## Repository layout

- [apps-manifest.json](/techofourown/sw-ourbox-apps-hello-world/apps-manifest.json)
  - machine-readable description of the published application
- [apps/hello-world](/techofourown/sw-ourbox-apps-hello-world/apps/hello-world)
  - source and image build inputs
- [.github/workflows/ci.yml](/techofourown/sw-ourbox-apps-hello-world/.github/workflows/ci.yml)
  - lightweight validation
- [.github/workflows/publish-images.yml](/techofourown/sw-ourbox-apps-hello-world/.github/workflows/publish-images.yml)
  - publishes the image to GHCR on `main`
