---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: compass.com
  spf: true
hosts:
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: www.compass.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Compass Real Estate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Compass, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Compass
provider_slug: compass-real-estate
slug: compass-real-estate-domain-security
source_filename: compass-real-estate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.compass.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: compass.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/compass-real-estate/refs/heads/main/security/compass-real-estate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real Estate
- Residential Real Estate
- Brokerage
- PropTech
- Real Estate Platform
- Agent Platform
- CRM
- Listings
- Compass One
- Compass AI
- Compass Lens
- Artificial Intelligence
- New York
---
