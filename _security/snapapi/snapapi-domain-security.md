---
api_specs:
- filename: openapi.json
  format: json
  label: SnapAPI
  slug: snapapi
  spec_type: OpenAPI
  url: https://snap.michaelcli.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: michaelcli.com
  spf: true
hosts:
- cert_expires: Sep  2 20:17:19 2026 GMT
  host: snap.michaelcli.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snapapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SnapAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: SnapAPI
provider_slug: snapapi
slug: snapapi-domain-security
source_filename: snapapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snap.michaelcli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:17:19 2026 GMT\n  hsts: false\ndomains:\n- domain: michaelcli.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snapapi/refs/heads/main/security/snapapi-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Screenshots
- Website Screenshots
- Metadata Extraction
- Text Extraction
- PDF Generation
- Headless Chromium
- Web Scraping
- Developer Tools
- REST
---
