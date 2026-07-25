---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: healthverity.com
  spf: true
hosts:
- cert_expires: Aug 26 04:58:20 2026 GMT
  host: healthverity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Healthverity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HealthVerity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: HealthVerity
provider_slug: healthverity
slug: healthverity-domain-security
source_filename: healthverity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: healthverity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 04:58:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: healthverity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthverity/refs/heads/main/security/healthverity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- United States
- Life Sciences
- Real-World Data
- Identity Resolution
- De-Identification
- Tokenization
- Data Marketplace
- HIPAA
- Claims
---
