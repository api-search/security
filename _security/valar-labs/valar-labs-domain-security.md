---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: valarlabs.com
  spf: false
hosts:
- cert_expires: Sep 22 08:27:10 2026 GMT
  host: www.valarlabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 08:45:46 2026 GMT
  host: portal.valarlabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Valar Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valar Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Valar Labs
provider_slug: valar-labs
slug: valar-labs-domain-security
source_filename: valar-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.valarlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 08:27:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.valarlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 08:45:46 2026 GMT\n  hsts: false\ndomains:\n- domain: valarlabs.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valar-labs/refs/heads/main/security/valar-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Oncology
- Cancer
- Diagnostics
- Artificial Intelligence
- Machine Learning
- Pathology
- Digital Pathology
- Precision Medicine
- HIPAA
---
