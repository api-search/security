---
api_specs:
- filename: freight-waves-sonar-openapi.yml
  format: yaml
  label: SONAR API
  slug: sonar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freight-waves/refs/heads/main/openapi/freight-waves-sonar-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freightwaves.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sonar.surf
  spf: true
hosts:
- cert_expires: Aug 25 08:44:54 2026 GMT
  host: freightwaves.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 09:55:36 2026 GMT
  host: api.sonar.surf
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:18:18 2026 GMT
  host: api.freightwaves.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freight Waves Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freight Waves, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Freight Waves
provider_slug: freight-waves
slug: freight-waves-domain-security
source_filename: freight-waves-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freightwaves.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 08:44:54 2026 GMT\n  hsts: false\n- host: api.sonar.surf\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 09:55:36 2026 GMT\n  hsts: false\n- host: api.freightwaves.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:18:18 2026 GMT\n  hsts: false\ndomains:\n- domain: freightwaves.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: sonar.surf\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freight-waves/refs/heads/main/security/freight-waves-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Freight
- Logistics
- Supply Chain
- Transportation
- Trucking
- Market Data
- Analytics
- Freight Rates
- SONAR
---
