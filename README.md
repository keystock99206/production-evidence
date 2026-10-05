# Production Evidence — Not Your Mama's Specialty Pages

Public certification records for digital artifacts released by
**Not Your Mama's Specialty Pages** — https://fold-blueprint-base.base44.app

Every artifact listed here is hash-pinned: its SHA-256 was computed from the
certified release binary and published here, so anyone can verify a file they
received without trusting anyone.

## Verify a file you received

**macOS**
```sh
shasum -a 256 <file>
```

**Linux**
```sh
sha256sum <file>
```

**Windows PowerShell**
```powershell
Get-FileHash <file>
```

**Windows Command Prompt**
```cmd
certutil -hashfile <file> SHA256
```

Compare the output against the hashes in [`SHA256SUMS`](SHA256SUMS).
If it matches, the file is byte-identical to the certified release.
If it differs, do not use the file.

## Published records

| Artifact | SHA-256 | Size | Distribution |
|---|---|---|---|
| JM-001 Bermuda customer package (digital release 001) | `1af230c274dfa3dcaab95ebe92ea6844336ffbccb54b794563e874d6aff2b594` | 46,769,210 bytes | Free download from the storefront |
| Proof Library 145 (composition proof PDF) | `6279997a6160eb99e3d75c003bd42dd6517a2b084fea47f1e60a7ef645eca848` | 1,070,508 bytes | Internal proof record — not distributed |

Machine-readable records live in [`artifacts/`](artifacts/).

## Rules of this record

- Paid artifacts publish their hash only — never their files.
- A record is added when an artifact is certified. Existing hashes are never
  edited; a changed artifact gets a new record.
- Hashes listed here were re-verified against the certified binaries on
  2026-10-05.
