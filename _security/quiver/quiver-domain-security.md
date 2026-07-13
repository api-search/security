---
api_specs:
- filename: quiver-openapi.yml
  format: yaml
  label: Quiver Quantitative API
  slug: quiver
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiver/refs/heads/main/openapi/quiver-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quiverquant.com
  spf: true
hosts:
- cert_expires: Oct  6 01:52:55 2026 GMT
  host: www.quiverquant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 01:52:55 2026 GMT
  host: api.quiverquant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quiver Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quiver Quantitative, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Quiver Quantitative
provider_slug: quiver
slug: quiver-domain-security
source_filename: quiver-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quiverquant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 01:52:55 2026 GMT\n  hsts: false\n- host: api.quiverquant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 01:52:55 2026 GMT\n  hsts: false\ndomains:\n- domain: quiverquant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quiver/refs/heads/main/security/quiver-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Alternative Data
- Financial Data
- Investment Research
- Market Data
- Government Data
- Congressional Trading
---
