---
api_specs:
- filename: api-documentation
  format: yaml
  label: pdflayer API
  slug: pdflayer-api
  spec_type: OpenAPI
  url: https://docs.apilayer.com/pdflayer/docs/api-documentation
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pdflayer.com
  spf: true
hosts:
- cert_expires: Oct  3 16:29:12 2026 GMT
  host: pdflayer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 19:00:24 2027 GMT
  host: api.pdflayer.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Pdflayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pdflayer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: pdflayer
provider_slug: pdflayer
slug: pdflayer-domain-security
source_filename: pdflayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pdflayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:29:12 2026 GMT\n  hsts: false\n- host: api.pdflayer.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  9 19:00:24 2027 GMT\n  hsts: false\ndomains:\n- domain: pdflayer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pdflayer/refs/heads/main/security/pdflayer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- PDF
- HTML to PDF
- Document Generation
- Web Capture
- APILayer
- PDF Conversion
---
