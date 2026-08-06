# Contributing to AIIS

The AI Injection and Infrastructure Signature Standard is authored in the open and published with a working reference implementation (the OpenA2A HoneyMap scanner). It is early, and we are looking for co-authors and contributors to help shape it before it goes to an external standards body. Your review, critique, and independent implementation work all carry weight on the spec.

## What we are looking for

- Review and critique. Read the [schema](schema/) and the existing [signatures](signatures/) and tell us where the format is ambiguous, where it leaves interoperability gaps, or where a signature is over-broad or imprecise.
- An independent second implementation. A non-HoneyMap engine that loads and matches AIIS signatures is the strongest signal that the format is sound and portable.
- Security audit and threat modeling of the spec itself, not just an implementation.
- Cryptography and signatures expertise, applied to detection-signature design. We want input from people who have built YARA rules, detection corpora, or injection and exposure fingerprints, and who can contribute high-precision, low-false-positive patterns. The corpus is intentionally conservative, so precision matters more than coverage.
- We need high-precision attack signatures and review from applied-cryptography researchers.

## Who we are looking for

We especially welcome:

- Security and cryptography researchers, including academic and PhD-level work.
- Standards-process experts (W3C, IETF, OpenTelemetry) who can help take these specifications to external bodies.
- Engineers building agent platforms and runtimes, for independent implementations and adoption.
- Red teamers and security auditors.

## How to contribute

- Open an issue or pull request on this repository.
- Or email info@opena2a.org with "co-author" in the subject line.
- For new attack signatures, injection research, or coordinated disclosure, email info@opena2a.org or info@opena2a.org.

Small fixes (typos, broken links, clarifications) can go straight to a pull request. For new signatures or changes to the signature schema, open an issue first so the change can be discussed and validated against the test corpus before implementation work begins.

## Ground rules

- Contributions are licensed under Apache-2.0, consistent with the project license.
- Be specific and evidence-based. A new signature should cite the artefact or exposure it matches and include a test case.
- No purely theoretical claims without a path to validation. Prefer high-precision patterns proven against real samples over broad patterns that raise false positives.
