# Reproduction of traces dashboard bug

## Start

```bash
docker compose up -d
```

See http://localhost:3000/d/tempo/tempo

![screen.png](screen.png)

The "No data" panel was added via "Add visualisation" menu on dashboard edit.

![edit-bad.png](edit-bad.png)

However, the traces are present in the "Explore" view.

![explore.png](explore.png)

The "Has data" panel was added from "Explore", "Add to dashboard" button.

![edit-good.png](edit-good.png)

## Cleanup

```bash
docker compose down --timeout 1
```
