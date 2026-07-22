---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pliantrx.com
  spf: true
hosts:
- cert_expires: Sep 15 01:49:01 2026 GMT
  host: pliantrx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pliant Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pliant Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pliant Therapeutics
provider_slug: pliant-therapeutics
slug: pliant-therapeutics-domain-security
source_filename: pliant-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pliantrx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:49:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pliantrx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pliant-therapeutics/refs/heads/main/security/pliant-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biopharmaceutical
- Pharmaceuticals
- Biotechnology
- Healthcare
- Clinical Trials
- Oncology
- Drug Discovery
- Life Sciences
---
