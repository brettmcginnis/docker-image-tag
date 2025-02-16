# docker-image-tag
Provides an image tag for pull requests or trunk

```yaml
  - uses: brettmcginnis/docker-image-tag@1.0.0
    id: docker

  - uses: docker/build-push-action@v3
    with:
      push: true
      tags: ${{ steps.docker.outputs.tag }}
```
