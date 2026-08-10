---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pathos.com
  spf: true
hosts:
- cert_expires: Sep 22 18:45:00 2026 GMT
  host: www.pathos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pathos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pathos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pathos
provider_slug: pathos
slug: pathos-domain-security
source_filename: pathos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pathos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 18:45:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pathos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pathos/refs/heads/main/security/pathos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Healthcare
- Biotechnology
- Oncology
- Drug Development
- Clinical Trials
- Precision Medicine
- Life Sciences
---
