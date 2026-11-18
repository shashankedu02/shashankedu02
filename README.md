# B S Shashank Aradhya

Information Science and Engineering undergraduate at The Oxford College of Engineering, Bengaluru.
I build **conservative, explainable verification tools on official Indian data**: tools that say only what they can
prove, show their evidence, and treat "unable to verify" as an honest answer.

## Selected work

| Project | What it does | Evidence |
|---|---|---|
| [**MedCheck**](https://github.com/shashankedu02/MedCheck) | Reads a medicine's batch number from a photo (local OCR) and checks it against CDSCO's *Not of Standard Quality* alert list. An alert needs an exact batch match plus product evidence; lookalike characters (O/0, I/1) make it abstain rather than guess. | 475 automated tests pass in CI on Ubuntu; the dataset rebuilds byte-for-byte from the official extraction. Real-photo results are reported separately and are explicitly *not* accuracy figures. |
| [**Asli Link**](https://github.com/shashankedu02/asli-link) | Checks whether a link really belongs to the Indian bank or government office it claims to be, using RBI's restricted `.bank.in` namespace and `.gov.in` as trust anchors, and explains each impersonation signal. | Registry cross-checked against Certificate Transparency logs (460 `.bank.in` domains); core and API tests run in CI on Python 3.11 and 3.13. |
| [**CloudDoctor**](https://github.com/shashankedu02/CloudDoctor) | Local static analyser for AWS IAM policies: explainable rules for privilege-escalation patterns, with IAM wildcard matching. | CI on every pull request; regression tests for the wildcard cases it used to miss. |
| [**APIWatch**](https://github.com/shashankedu02/APIWatch) | On-demand HTTP endpoint checks with an SSRF guard that re-validates every redirect. | Small FastAPI + React tool. |

## How I work

- Every claim in a README should be something a test or a recorded run can show. Limitations are part of the product.
- I use AI coding tools, and I treat their output like any other code: reviewed, tested in CI and documented, never
  taken on trust.
- Python first. FastAPI for services, React + TypeScript when a UI needs it, pytest and GitHub Actions for everything.

## Hackathons and recognition

- **Smart India Hackathon 2026:** qualified Round 1; Round 2 submission completed.
- **Bengaluru Tech Summit 2026 Hackathon:** qualified Round 1.
- **Viksit Bharat Young Leaders Dialogue 2027:** first place in the Tumakuru district championship.
- **NDA 2024:** qualified the written exam and reached the SSB (five-day) stage. NCC cadet.

## Contact

[LinkedIn](https://www.linkedin.com/in/shashank-aradhya-aa3516442/)
