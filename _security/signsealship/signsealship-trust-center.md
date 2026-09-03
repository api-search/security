---
api_specs:
- filename: openapi.json
  format: json
  label: SignSealShip Partner API
  slug: partner-api
  spec_type: OpenAPI
  url: https://docs.signsealship.com/api-reference/openapi.json
certifications:
- count
- named
- note
description: ''
kind: trust-center
layout: security
name: Signsealship Trust Center
name_suffix: Trust Center
overview: SignSealShip Partner API maintains a public trust center documenting count, named, and note compliance.
provider_name: SignSealShip Partner API
provider_slug: signsealship
slug: signsealship-trust-center
source_filename: signsealship-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: https://signsealship.com/security\ndocs: https://signsealship.com/security\nprobed: '2026-09-01'\nhttp_status: 200\ntrust_center:\n  published: true\n  url: https://signsealship.com/security\n  title: Security & Trust\n  self_description: Trust center\n  linked_as: Linked as \"Trust Center\" in the site header and footer navigation\ncertifications:\n  count: 0\n  named: []\n  note: >-\n    NO CERTIFICATIONS ARE HELD OR CLAIMED. This is recorded as a genuine zero, not as a gap in\n    our reading. The page publishes an explicit \"honest table\" of what is and is not built,\n    headed \"If it isn't marked 'built in' here, we don't claim it anywhere.\"\nhonest_table:\n- item: ESIGN Act (15 U.S.C. 7001)\n  status: built in\n  detail: >-\n    Consent captured per 101(c) before any signing; signatures attributed to identified signers;\n    records retained and reproducible.\n- item: UETA\n  status: built in\n  detail: Intent, attribution\
  \ and record integrity handled by the signing flow and audit trail.\n- item: Tamper-evident sealing (CMS / PKCS#7)\n  status: built in\n  detail: >-\n    Every sealed PDF carries a cryptographic signature verifiable in Adobe Acrobat with no\n    SignSealShip account.\n- item: SHA-256 tamper-evident audit trail\n  status: built in\n  detail: Append-only event log per envelope; each event chains to the previous one.\n- item: RON state rules\n  status: built in\n  detail: >-\n    Deterministic state-and-document rules checked before payment; restricted combinations are\n    refused.\n- item: SOC 2 Type II\n  status: on roadmap\n  detail: >-\n    \"Not yet certified, and we won't imply otherwise.\" No date is claimed pending an auditor.\n- item: ISO 27001\n  status: not certified\n  detail: '\"We don''t hold this certification and don''t claim it.\"'\ncontrols_published:\n  document_integrity: >-\n    Asymmetric signing key held in Google Cloud KMS; the private key never leaves Google's\n\
  \    infrastructure. A hash of the finished PDF is signed and the CMS (PKCS#7) signature is\n    embedded covering the PDF ByteRange, so a single changed byte visibly breaks the seal in any\n    standards-compliant validator -- verifiable on the reader's own machine.\n  audit_trail: >-\n    Append-only event log; each event carries the SHA-256 of the event before it. CONSENT /\n    VIEWED / SIGNED / SEALED events recorded in UTC with originating IP.\n  identity_verification: >-\n    Knowledge-based authentication from public records plus government-ID credential analysis,\n    then a live state-commissioned notary on camera. RON available through notaries in 43\n    jurisdictions.\n  encryption: >-\n    TLS on every path in transit; encrypted at rest on Google Cloud. Customer document buckets\n    block all public access; signing links expire 24 hours after issue; time-limited signed URLs\n    used only where a delivery rail requires them.\n  retention: Sealed documents kept in a dedicated\
  \ 7-year retention bucket.\n  infrastructure: >-\n    Cloud Run, Cloud SQL (managed PostgreSQL) and Cloud KMS. Each deployed service runs under its\n    own dedicated service account with least-privilege access. Secrets mounted from a managed\n    secret store, never baked into images. Deploys ship by immutable image digest with the source\n    commit verifiable at https://signsealship.com/api/version.\n  edge: >-\n    Cloudflare in front of public /api/* traffic with an origin shared-secret check and rate\n    limits on every public write.\n  inbound_webhooks: >-\n    Fail closed -- every inbound vendor event must pass signature verification, and if a vendor's\n    verification is not configured its route does not exist in production.\n  data_handling: >-\n    Uploads are malware-scanned (event-driven ClamAV) and DLP-classified with category names only\n    -- never content -- in logs.\nsubprocessors:\n  published: true\n  disclosure_level: by role, not by name\n  named_directly:\n  -\
  \ Google Cloud Platform\n  - Stripe\n  by_role:\n  - Remote online notarization network partner\n  - Shipping API partner (USPS, UPS, FedEx labels and tracking)\n  - Print-and-mail fulfillment partner\n  - Transactional email provider\n  note: >-\n    Business customers can request the fully named subprocessor list under a data-processing\n    agreement. Partial naming is a real limitation for a vendor-review process, and the page says\n    so rather than hiding it.\nverifiability_claim: >-\n  The distinguishing posture of this trust center is that its central security claim is\n  independently checkable by the reader without trusting the vendor: open a sealed PDF in free\n  Adobe Reader and inspect the signature panel. Very few trust centers of any size offer a\n  reader-executable proof in place of a badge.\ngaps:\n- No SOC 2, ISO 27001 or any third-party attestation.\n- No named subprocessor list without a DPA.\n- No /.well-known/security.txt -- see security/signsealship-vulnerability-disclosure.yml.\n\
  - No penetration-test summary or architecture attestation published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signsealship/refs/heads/main/security/signsealship-trust-center.yml
summary_line: count, named, note
tags:
- notarization
- remote online notarization
- electronic signature
- document verification
- legal technology
- real estate
- title and escrow
- shipping
trust_url: ''
---
