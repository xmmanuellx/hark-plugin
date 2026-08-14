<!--
Fork empaquetado de Hark con proveedores OpenAI-compatibles personalizables.
Generado con scripts/package-plugin.sh desde xmmanuellx/hark.
-->

# Hark (Omarchy plugin) — fork de xmmanuellx

Fork de [Hark](https://github.com/konradk/hark) que añade **proveedores
OpenAI-compatibles con base URL personalizable**, configurables desde el
panel de ajustes, `config.lua` y la CLI.

Construido desde `xmmanuellx/hark@51d2170`. El PR original está en
https://github.com/konradk/hark/pull/1.

```bash
omarchy plugin add https://github.com/xmmanuellx/hark-plugin.git --enable
omarchy-shell shell summon hark
```

Actualiza con `omarchy plugin update hark`.

## Qué añade este fork

- Sección **Providers** en los ajustes (`Ctrl+,`): añade/edita/elimina
  endpoints OpenAI-compatibles (name, base URL y API key).
- **Varios modelos por proveedor**: cada modelo usa su id del endpoint como
  nombre (no hace falta nombrarlo) y puedes añadirlos/quitarlos.
- **Fetch de modelos**: lista los modelos que expone el endpoint
  (`GET {base_url}/models`) y añádelos con un clic.
- Tabla `providers` en `~/.config/hark/config.lua`.
- Comandos `harkctl provider list/add/remove/fetch-models` y
  `harkctl model add/remove`.
- Los binarios estáticos `harkd`/`harkctl` ya están incluidos (no hace falta Go).

## License

[MIT](LICENSE).
