---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tishmanspeyer.com
  spf: true
hosts:
- cert_expires: Sep 21 02:46:15 2026 GMT
  host: www.tishmanspeyer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tishman Speyer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tishman Speyer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tishman Speyer
provider_slug: tishman-speyer
slug: tishman-speyer-domain-security
source_filename: tishman-speyer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tishmanspeyer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 02:46:15 2026 GMT\n  hsts: null\ndomains:\n- domain: tishmanspeyer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tishman-speyer/refs/heads/main/security/tishman-speyer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Asset Management
- Commercial Real Estate
- Coworking
- Investment Management
- Life Sciences Real Estate
- Mixed-Use Development
- Office
- Property Management
- Proptech
- Real Estate
- Real Estate Development
- Residential
- Tenant Experience
---
