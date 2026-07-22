---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apprentice.io
  spf: true
hosts:
- cert_expires: Oct  8 18:50:50 2026 GMT
  host: www.apprentice.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Apprentice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apprentice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apprentice
provider_slug: apprentice
slug: apprentice-domain-security
source_filename: apprentice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apprentice.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 18:50:50 2026 GMT\n  hsts: false\ndomains:\n- domain: apprentice.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apprentice/refs/heads/main/security/apprentice-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Healthcare
- Life Sciences
- Pharmaceutical
- Manufacturing
- Manufacturing Execution System
- Cloud
- GxP
- Quality
---
