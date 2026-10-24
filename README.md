# Movimientos de Wallet

Herramienta web sencilla para llevar la contabilidad de **todo lo que entra y sale** de una
wallet de criptomonedas, mostrado en **euros** y con lenguaje claro (pensada para alguien que
no sabe de crypto).

Consulta datos públicos de la blockchain (los mismos que verías en **Etherscan** y
**Basescan**) a través de la API pública de Blockscout. No guarda nada en ningún servidor y no
pide claves: es un único archivo HTML.

## Qué hace

- Pides la dirección de la wallet (`0x…`).
- Ves **Entradas y Salidas** con el importe en €, de dónde viene / a dónde va y la plataforma
  (Coinbase, Binance, etc.).
- Resumen de **Entró / Salió / Balance** del periodo.
- Filtros: periodo (7/30/90 días o todo), redes (Ethereum y Base por defecto; Arbitrum,
  Polygon y zkSync opcionales) y tipo (Todo / Entradas / Salidas).
- **Buscar por ID de transacción**, dirección o plataforma.
- **Copiar** cada movimiento o toda la lista (para pegar en Excel/Sheets o WhatsApp).
- Oculta y avisa de **tokens falsos sin valor** (estafa de *address poisoning*).

## Cómo usarla

### Opción A — Abrir online (la más fácil, no se descarga nada)

Si está activado GitHub Pages, solo hay que abrir este enlace en el navegador:

```
https://0xhexx1.github.io/movimientos-wallet/
```

### Opción B — Descargarla y abrirla en el ordenador

1. En la página del repositorio, pulsa el botón verde **« Code »** → **« Download ZIP »**.
2. Descomprime el ZIP.
3. Doble clic en **`index.html`** → se abre en tu navegador.

No hace falta instalar nada. Solo necesita conexión a internet (consulta la blockchain en vivo).

### Opción C — Clonar con git

```bash
git clone https://github.com/0xHexX1/movimientos-wallet.git
cd movimientos-wallet
# doble clic en index.html, o:
open index.html        # macOS
```

## Notas

- Importes en € calculados al cambio actual (aproximado). No incluye comisiones de red (gas).
- Nunca copies una dirección desde el historial para reutilizarla: cópiala siempre de la
  fuente oficial (por la estafa de *address poisoning*).
