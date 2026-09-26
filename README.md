# Density Opaque

Density Opaque is an independent protocol in the Quant/Qudit architecture. It is **not** a fifth lifecycle color.

The core model remains:

`RED scope geometry + RED/BLUE/YELLOW/BLACK lifecycle + Density Opaque protocol + WHITE projection`

## YELLOW — operational opacity

A YELLOW Acted Token may temporarily enable Density Opaque while an authorized edit or processing lease is active. External mutation is restricted to prevent collisions while safe metadata, health, lifecycle, project scope, and lease status remain observable.

Operational opacity is reversible and does not seal the Quant.

## BLACK — structural opacity

A legitimately completed BLACK Token derives permanent structural opacity from its cryptographic seal. BLACK immutability remains the integrity mechanism; Density Opaque controls what the WHITE `shadeQudit()` projection exposes.

The underlying sealed history is not destroyed merely to make it opaque. Authorized storage retains the sealed record while presentation/access policy can expose identity, topic, enclosure lineage, timestamps, public catalog metadata, and the SHA-256 seal without exposing protected internals.

## Suggested schema

```json
{
  "protocols": {
    "densityOpaque": {
      "enabled": true,
      "mode": "operational",
      "reason": "active-processing",
      "since": "ISO-8601 timestamp",
      "leaseId": "optional"
    }
  }
}
```

Allowed modes are `operational` for temporary YELLOW isolation and `structural` for BLACK sealed projection. External APIs cannot use Density Opaque to manufacture lifecycle authority or bypass Monitor/Cloudlair sealing rules.
