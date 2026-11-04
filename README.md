# sample-reqif-doors-next

Public ReqIF sample in the shape of IBM DOORS Next exports, with the
**fidelity receipt** [Traceo](https://traceo.cloud) writes when it reads it.

> **Read this first.** At least one file here is *shaped*: hand-written to resemble an export from IBM DOORS Next, not produced by it. A clean read of a shaped file shows that Traceo reads that shape. It does not show that Traceo reads what the tool really emits.

## Files

| File | Kind | Source | Licence | sha256 (prefix) |
|---|---|---|---|---|
| `doors_next_shaped.reqif` | **shaped**: hand-written to look like the tool's export, *not* produced by it | [`jackhale98/sysml-web`](https://github.com/jackhale98/sysml-web/blob/cddbd21/src/lib/dataio/fixtures/reqif/doors-next.reqif) @ `cddbd21` | Apache-2.0 OR MIT | `d6391ee17b72a495` |

- `doors_next_shaped.reqif`: Hand-written in the shape of a DOORS Next export (`jazz.example.com` repository, 2026 timestamps). DOORS Next did not produce it.

Each file is copied byte-for-byte from the repository named and is unedited. Check it against the sha256.

## What Traceo kept

Traceo writes a receipt before it imports anything. The receipt counts every class of item **in**
the file and **kept**. It names every item it did not keep, with a reason code. A file with nothing
in it gets the verdict `vacuous`, never `clean`.

### `doors_next_shaped.reqif`

Verdict: **clean**, every item in the file was kept.

| Class | In the file | Kept |
|---|---:|---:|
| objects | 7 | 7 |
| attributes | 26 | 26 |
| enumeration values | 9 | 9 |
| link types | 2 | 2 |
| links | 3 | 3 |
| hierarchy nodes | 7 | 7 |

Full receipt: [`receipts/doors_next_shaped.reqif.receipt.json`](receipts/doors_next_shaped.reqif.receipt.json)

These receipts were written by Traceo's ReqIF importer at commit `90cfc15` on 2026-11-03.

## Try it

[Sign up](https://app.traceo.cloud/signup), open Import and choose a file from this repository. Traceo
shows its receipt before anything is written.

## Names

IBM DOORS Next is a trademark of its owner. It is named here only to describe the file. Traceo is not
affiliated with or endorsed by its owner.

## Licence

The `.reqif` files are third-party and keep their upstream licence. The texts are in
[`LICENSES/`](LICENSES/). The README and the `receipts/` are © Traceo, released under the MIT
licence in [`LICENSE`](LICENSE).
