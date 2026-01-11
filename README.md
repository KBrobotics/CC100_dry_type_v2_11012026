# Industrial Transformer Dashboard (WAGO CC100)

Lekki, przemysłowy dashboard HMI do monitoringu transformatorów suchych.

## Szybki Start (Portainer):
1. Skopiuj zawartość pliku `docker-compose.yml`.
2. W Portainerze: **Stacks** -> **Add stack** -> Wklej kod -> **Deploy**.
3. Dashboard ruszy na porcie **8000** sterownika.

## Konfiguracja:
- **Adres URL**: `http://<HOST_IP>:8000`
- **Node-RED**: Zaimportuj plik `node-red-flow.json`. 
- **WebSocket**: Dashboard łączy się domyślnie z `ws://<HOST_IP>:1880/ws/transformer`.

## Struktura:
- `App.tsx` - logika aplikacji i WebSocket.
- `components/` - wizualizacje SVG.
- `node-red-flow.json` - gotowy przepływ do sterownika.
- `docker-compose.yml` - konfiguracja kontenera.
