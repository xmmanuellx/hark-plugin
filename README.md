<!--
Fork empaquetado de Hark con proveedores OpenAI-compatibles personalizables.
Generado con scripts/package-plugin.sh desde xmmanuellx/hark.
-->

# Hark (Omarchy plugin) — fork de xmmanuellx

Fork de [Hark](https://github.com/konradk/hark) que añade **proveedores
OpenAI-compatibles con base URL personalizable**, configurables desde el
panel de ajustes, `config.lua` y la CLI.

Construido desde `xmmanuellx/hark@80accfd`. El PR original está en
https://github.com/konradk/hark/pull/1.

```bash
omarchy plugin add https://github.com/xmmanuellx/hark-plugin.git --enable
omarchy-shell shell summon hark
```

Actualiza con `omarchy plugin update hark`.

## Qué añade este fork

- Sección **Providers** en los ajustes (`Ctrl+,`): añade/edita/elimina
  endpoints OpenAI-compatibles (name, base URL y API key).
- **Varios modelos por proveedor**: escribe el id del modelo y pulsa
  **Add model**; cada modelo usa su id como nombre (no hay que nombrarlo).
- Tabla `providers` en `~/.config/hark/config.lua`.
- Comandos `harkctl provider list/add/remove` y `harkctl model add/remove`.
- Los binarios estáticos `harkd`/`harkctl` ya están incluidos (no hace falta Go).

## License

[MIT](LICENSE).
