---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ringtx.com
  spf: true
hosts:
- cert_expires: Sep 18 23:14:38 2026 GMT
  host: ringtx.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ring Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ring Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ring Therapeutics
provider_slug: ring-therapeutics
slug: ring-therapeutics-domain-security
source_filename: ring-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ringtx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:14:38 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: ringtx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ring-therapeutics/refs/heads/main/security/ring-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Gene Therapy
- Life Sciences
- Pharmaceuticals
- Research
- Flagship Pioneering
---
