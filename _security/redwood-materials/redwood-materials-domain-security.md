---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: redwoodmaterials.com
  spf: true
hosts:
- cert_expires: Oct  2 09:38:09 2026 GMT
  host: www.redwoodmaterials.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 21:44:16 2026 GMT
  host: portal.redwoodmaterials.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 2592000
  https: true
  note: gated AWS Cognito partner portal (auto-recycler battery pack sales); no public API
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Redwood Materials Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redwood Materials, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Redwood Materials
provider_slug: redwood-materials
slug: redwood-materials-domain-security
source_filename: redwood-materials-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.redwoodmaterials.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 09:38:09 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: portal.redwoodmaterials.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 21:44:16 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  hsts_include_subdomains: true\n  note: gated AWS Cognito partner portal (auto-recycler battery pack sales); no public API\ndomains:\n- domain: redwoodmaterials.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redwood-materials/refs/heads/main/security/redwood-materials-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Battery Recycling
- Critical Minerals
- Energy Storage
- Electric Vehicles
- Circular Economy
- Manufacturing
- Supply Chain
- Sustainability
- Cleantech
- Materials
---
