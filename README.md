# DID documents for the thesis PoC

GitHub Pages hosts the `did:web` DID documents of the two PoC issuers. The
code lives in a separate private repository.

| DID | Resolves to |
| --- | --- |
| `did:web:chrysa712.github.io:thesis-did:build` | https://chrysa712.github.io/thesis-did/build/did.json |
| `did:web:chrysa712.github.io:thesis-did:scan` | https://chrysa712.github.io/thesis-did/scan/did.json |

Each document holds one public EC P-256 key (`assertionMethod`), which
verifiers use to check the issuer's credentials, and a `TokenStatusList`
service with the issuer's status list endpoint. The private keys never
appear in this repository.

The status list endpoints point to `127.0.0.1` because the PoC issuers run
inside the CI job that uses them.
