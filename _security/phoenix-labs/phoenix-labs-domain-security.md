---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: phxlabs.ca
  spf: true
hosts:
- cert_expires: Aug 27 15:13:36 2026 GMT
  host: phxlabs.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phoenix Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phoenix Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Phoenix Labs
provider_slug: phoenix-labs
slug: phoenix-labs-domain-security
source_filename: phoenix-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: phxlabs.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 15:13:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: phxlabs.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phoenix-labs/refs/heads/main/security/phoenix-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Video Games
- Game Development
- Entertainment
- Online Games
---
