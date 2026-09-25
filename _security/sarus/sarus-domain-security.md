---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sarus.tech
  spf: true
hosts:
- cert_expires: Dec  2 08:44:55 2026 GMT
  host: www.sarus.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: docs.sarus.tech
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''docs.sarus.'
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Sarus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sarus, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sarus
provider_slug: sarus
slug: sarus-domain-security
source_filename: sarus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sarus.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 08:44:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sarus.tech\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''docs.sarus.'\n  hsts: null\ndomains:\n- domain: sarus.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sarus/refs/heads/main/security/sarus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Data
- Privacy
- Differential Privacy
- Synthetic Data
- Analytics
- Machine Learning
- Data Governance
- SQL
- Open Source
---
