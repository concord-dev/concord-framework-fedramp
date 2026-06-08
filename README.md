# concord-framework-fedramp

FedRAMP Moderate Baseline framework manifest for Concord. Install via:

```sh
concord add fedramp
```

Pulls in `concord-controlpack-fedramp` (NIST 800-53 Rev 5 controls
selected by the FedRAMP Moderate baseline, with FedRAMP overlays).

## Source

Baseline mappings are drawn from
[usnistgov/oscal-content](https://github.com/usnistgov/oscal-content)
FedRAMP profiles and GSA's published baselines. Every control's rego
references the official NIST OSCAL catalog identifier in its
`metadata.id` so OSCAL component-definition export round-trips cleanly.

## Coverage

v0.1.0 ships a core baseline. Subsequent releases expand to full
parity with the FedRAMP Moderate control set as the underlying OPA
rules mature.
