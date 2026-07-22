---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: torchdental.com
  spf: true
hosts:
- cert_expires: Sep  4 15:05:02 2026 GMT
  host: torchdental.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Torchdental Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Torchdental, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Torchdental
provider_slug: torchdental
slug: torchdental-domain-security
source_filename: torchdental-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: torchdental.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:05:02 2026 GMT\n  hsts: false\ndomains:\n- domain: torchdental.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/torchdental/refs/heads/main/security/torchdental-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Dental
- Healthcare
- Procurement
- E-Commerce
- Supply Chain
- B2B
- SaaS
---
