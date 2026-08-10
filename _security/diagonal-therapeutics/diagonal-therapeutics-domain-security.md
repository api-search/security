---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: diagonaltx.com
  spf: true
hosts:
- cert_expires: Oct  4 18:43:47 2026 GMT
  host: diagonaltx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Diagonal Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diagonal Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Diagonal Therapeutics
provider_slug: diagonal-therapeutics
slug: diagonal-therapeutics-domain-security
source_filename: diagonal-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: diagonaltx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 18:43:47 2026 GMT\n  hsts: null\ndomains:\n- domain: diagonaltx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diagonal-therapeutics/refs/heads/main/security/diagonal-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Therapeutics
- Antibodies
- Drug Discovery
- Rare Disease
- Clinical Trials
- Life Sciences
- Pharmaceuticals
- United States
---
