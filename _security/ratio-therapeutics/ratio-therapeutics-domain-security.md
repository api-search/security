---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ratiotx.com
  spf: true
hosts:
- cert_expires: Nov  6 12:41:36 2026 GMT
  host: ratiotx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ratio Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ratio Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ratio Therapeutics
provider_slug: ratio-therapeutics
slug: ratio-therapeutics-domain-security
source_filename: ratio-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ratiotx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 12:41:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ratiotx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ratio-therapeutics/refs/heads/main/security/ratio-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Healthcare
- Oncology
- Radiopharmaceuticals
- Drug Discovery
- Clinical Trials
- Precision Medicine
---
