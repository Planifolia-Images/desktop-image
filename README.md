# Planifolia Desktop Image

Containerfile for building a Planifolia Desktop image.

This image is based on `nisel11/core` and offers GNOME.

> [!CAUTION]
> This image is experimental and isn't suitable for production. If you encounter any bugs during testing, please report them in this repository.

## Build

> [!NOTE]
> The fsguard compiled plugin `.so` file should be downloaded from the [latest release](https://github.com/Vanilla-OS/vib-fsguard/releases/latest) and be placed under a `plugins` directory beside the `recipe.yml` file.

```bash
vib build recipe.yml
podman image build -t planifolia/desktop .
```
