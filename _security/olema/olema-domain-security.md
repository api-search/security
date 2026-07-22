---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: olema.com
  spf: true
hosts:
- cert_expires: Sep  7 06:40:14 2026 GMT
  host: www.olema.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Olema Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Olema, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Olema
provider_slug: olema
slug: olema-domain-security
source_filename: olema-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.olema.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 06:40:14 2026 GMT\n  hsts: false\ndomains:\n- domain: olema.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olema/refs/heads/main/security/olema-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biopharmaceutical
- Oncology
- Healthcare
- Pharmaceuticals
- Clinical Trials
- Life Sciences
- Breast Cancer
---
