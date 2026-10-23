# ecw-poc-jwks

Public JWKS (public key only) for the Omilia OCP <-> eClinicalWorks POC backend app
(SMART Backend Services, RS384, `kid: ecw-poc-1`).

- URL to register with eCW: `https://jliddar-omilia.github.io/ecw-poc-jwks/jwks.json`
- The private key never leaves the broker host. This repo holds no secrets and no patient data.
- Rotate: generate a new key in the broker repo (`make keys`), add the new public key here
  alongside the old one, then remove the old one after eCW has picked up the change.

Owner: Omilia Natural Language Solutions (internal POC). Same pattern as `epic-poc-jku` (decision D-003).
