# RedAssistance — Brand Assets

Megosztott brand tokenek és design-rendszer-elemek minden RedAssistance design-hoz.

## Fájlok

| Fájl | Cél |
|---|---|
| `colors_and_type.css` | CSS custom properties: színek, fontok, rádiusz, árnyékok, layout |

## Használati szabály

**A `live/*/index.html`-ekben mindent INLINE-OLNI kell.** A self-contained követelmény miatt egyetlen design sem hivatkozhat relatív útvonalon erre az `assets/` mappára — mert a Pages routing nem feltétlenül oldja jól a `../../assets/...` útvonalakat minden mély URL-nél.

### Workflow

1. Frissítsd itt a master token-eket
2. Másold a `:root { ... }` blokk tartalmát az új design `<style>` blokk legtetejére
3. Bumppold a design `meta.yaml` `version`-jét
4. Frissítsd a `_index.md` katalógust ha státusz változik

## Brand alaprajz

- **Piros:** `#E11D2E` (saját RedAssistance vörös — NE kombinálj Bosch-logóval, az licenc-ütközést okozhat)
- **Font:** Geist + Geist Mono (Vercel család — Google Fonts CDN-en elérhető)
- **Sarok-rádiusz:** 6 / 10 / 16 / 24 px (sm / md / lg / xl)
- **Tinta-hierarchia:** 3 szint (ink #0A0A0A → muted #4A4A4A → light #6B6B6B)

## Verziók

- **v1** — 2026-05-22 — Initial release a `sezonier-roti` landing oldallal
