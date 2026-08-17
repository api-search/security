---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rhapsody.health
  spf: true
  spf_note: The automated probe returned spf:false on 2026-08-14; verified by hand the same day with `dig +short TXT rhapsody.health`, which does return "v=spf1 mx ip4:54.240.69.246/32 ip4:54.240.69.247/32 ...". The domain publishes 32 TXT records and the probe's lookup truncated, so the false was a probe artifact, not a missing record. Corrected to true.
hosts:
- cert_expires: Nov  8 10:54:11 2026 GMT
  host: rhapsody.health
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rhapsody Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rhapsody, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rhapsody
provider_slug: rhapsody
slug: rhapsody-domain-security
source_filename: rhapsody-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rhapsody.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 10:54:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: rhapsody.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  spf_note: >-\n    The automated probe returned spf:false on 2026-08-14; verified by hand the\n    same day with `dig +short TXT rhapsody.health`, which does return\n    \"v=spf1 mx ip4:54.240.69.246/32 ip4:54.240.69.247/32 ...\". The domain\n    publishes 32 TXT records and the probe's lookup truncated, so the false was a\n    probe artifact, not a missing record. Corrected to true.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhapsody/refs/heads/main/security/rhapsody-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- United States
- Interoperability
- Integration Engine
- FHIR
- HL7
- EMPI
- Terminology
- Health Data
- MCP
- API Gateway
---
