<!--
Fork empaquetado de Hark con proveedores OpenAI-compatibles personalizables.
Generado con scripts/package-plugin.sh desde xmmanuellx/hark.
-->

# Hark (Omarchy plugin) — fork de xmmanuellx

Fork de [Hark](https://github.com/konradk/hark) que añade **proveedores
OpenAI-compatibles con base URL personalizable**, configurables desde el
panel de ajustes, `config.lua` y la CLI.

Construido desde `xmmanuellx/hark@279787a`. El PR original está en
https://github.com/konradk/hark/pull/1.

```bash
omarchy plugin add https://github.com/xmmanuellx/hark-plugin.git --enable
omarchy-shell shell summon hark
```

Actualiza con `omarchy plugin update hark`.

## Qué añade este fork

- Sección **Providers** en los ajustes (`Ctrl+,`): añade/elimina endpoints
  OpenAI-compatibles (name, base URL, model ID y API key) sin tocar archivos.
- Tabla `providers` en `~/.config/hark/config.lua`.
- Comandos `harkctl provider list/add/remove`.
- Los binarios estáticos `harkd`/`harkctl` ya están incluidos (no hace falta Go).

## License

[MIT](LICENSE).
