---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rivia.com
  spf: true
hosts:
- cert_expires: Sep 29 00:48:18 2026 GMT
  host: www.rivia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rivia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rivia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rivia
provider_slug: rivia
slug: rivia-domain-security
source_filename: rivia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rivia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 00:48:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rivia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rivia/refs/heads/main/security/rivia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Clinical Trials
- Healthcare
- Life Sciences
- Data Intelligence
- Pharmaceutical
- Artificial Intelligence
- Clinical Data Management
---
