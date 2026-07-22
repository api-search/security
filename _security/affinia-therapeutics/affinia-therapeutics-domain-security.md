---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: affiniatx.com
  spf: true
hosts:
- cert_expires: Oct  6 11:29:41 2026 GMT
  host: affiniatx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Affinia Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Affinia Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Affinia Therapeutics
provider_slug: affinia-therapeutics
slug: affinia-therapeutics-domain-security
source_filename: affinia-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: affiniatx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 11:29:41 2026 GMT\n  hsts: false\ndomains:\n- domain: affiniatx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affinia-therapeutics/refs/heads/main/security/affinia-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Gene Therapy
- AAV
- Rare Disease
- Cardiology
- Pharmaceuticals
- Clinical Stage
---
