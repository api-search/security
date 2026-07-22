---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: forus.com
  spf: true
hosts:
- cert_expires: Oct  4 13:39:16 2026 GMT
  host: forus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Forus Fka Tandem Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forus (fka Tandem Health), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Forus (fka Tandem Health)
provider_slug: forus-fka-tandem-health
slug: forus-fka-tandem-health-domain-security
source_filename: forus-fka-tandem-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 13:39:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: forus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forus-fka-tandem-health/refs/heads/main/security/forus-fka-tandem-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Prior Authorization
- Medication Access
- Artificial Intelligence
- Health IT
- HIPAA
- Pharmacy
---
