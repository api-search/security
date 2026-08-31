---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: ardatherapeutics.com
  spf: true
hosts:
- cert_expires: Sep 23 09:07:44 2026 GMT
  host: ardatherapeutics.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arda Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arda Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Arda Therapeutics
provider_slug: arda-therapeutics
slug: arda-therapeutics-domain-security
source_filename: arda-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ardatherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:07:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ardatherapeutics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arda-therapeutics/refs/heads/main/security/arda-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Biotechnology
- Therapeutics
- Cell Depletion
- Single-Cell
- Drug Discovery
- Life Sciences
- Healthcare
---
