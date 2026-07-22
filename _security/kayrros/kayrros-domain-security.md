---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kayrros.com
  spf: true
hosts:
- cert_expires: Sep 12 23:58:51 2026 GMT
  host: www.kayrros.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kayrros Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kayrros, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kayrros
provider_slug: kayrros
slug: kayrros-domain-security
source_filename: kayrros-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kayrros.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:58:51 2026 GMT\n  hsts: null\ndomains:\n- domain: kayrros.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kayrros/refs/heads/main/security/kayrros-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data
- Geospatial
- Satellite Imagery
- Energy
- Environmental Intelligence
- Emissions
- Methane
- Analytics
- Climate
- Machine Learning
---
