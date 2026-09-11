---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: candeltx.com
  spf: true
hosts:
- cert_expires: Dec  6 18:31:36 2026 GMT
  host: candeltx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Candel Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Candel Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Candel Therapeutics
provider_slug: candel-therapeutics
slug: candel-therapeutics-domain-security
source_filename: candel-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: candeltx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 18:31:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: candeltx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/candel-therapeutics/refs/heads/main/security/candel-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Immunotherapy
- Oncology
- Life Sciences
- Clinical Trials
- Healthcare
---
