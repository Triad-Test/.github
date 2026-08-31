# Organization Resident Runtime / Interlock-InTr Handoff

Organization: **Triad-Test**  
Runtime owner: **Triad-Test/.github**

All Triad-Test resident-runtime activation declarations and organization-boundary
ingress/egress mechanisms are owned by this `.github` repository.

Sibling repositories may supply application payloads, models, formal tests,
documents, or handlers, but may not become an alternate organization runtime
owner or bypass this Interlock/InTr boundary.

```text
Triad-Test application/work repo
  -> Triad-Test/.github
  -> Interlock
  -> governed InTr packet
  -> HB / deterministic HB-derived carrier when available
  -> receiving Interlock
```

Machine surfaces:
- `control/organization-runtime.json`
- `runtime/organization_runtime.py`
- `runtime/activations/`
- `runtime/egress/`
- `runtime/ingress/`

HB, derived carriers, and InTr grant no execution, credential, routing,
transition, publication, or receiving authority. Credential authority remains
TV/TVC. GitHub Actions may validate source/evidence but is not the resident runtime.
