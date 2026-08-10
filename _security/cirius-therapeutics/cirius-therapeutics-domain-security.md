---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ciriustx.com
  spf: true
hosts:
- cert_expires: Nov 18 17:24:56 2026 GMT
  host: ciriustx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cirius Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cirius Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cirius Therapeutics
provider_slug: cirius-therapeutics
slug: cirius-therapeutics-domain-security
source_filename: cirius-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ciriustx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 17:24:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ciriustx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cirius-therapeutics/refs/heads/main/security/cirius-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Pharmaceuticals
- Biotechnology
- Life Sciences
- Healthcare
- Clinical Trials
- Metabolic Disease
- Diabetes
---
