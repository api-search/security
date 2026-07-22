---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: engieimpact.com
  spf: true
hosts:
- cert_expires: Oct  3 02:48:22 2026 GMT
  host: www.engieimpact.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Engie Insight Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ENGIE Insight Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ENGIE Insight Services
provider_slug: engie-insight-services
slug: engie-insight-services-domain-security
source_filename: engie-insight-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.engieimpact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:48:22 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: engieimpact.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/engie-insight-services/refs/heads/main/security/engie-insight-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Sustainability
- Resource Management
- Utilities
- Data Management
- Consulting
- Decarbonization
---
