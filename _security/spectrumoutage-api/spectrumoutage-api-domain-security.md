---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: SpectrumOutage API v1
  slug: spectrumoutage-api-v1
  spec_type: OpenAPI
  url: https://api.spectrumoutage.us/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spectrumoutage.us
  spf: true
hosts:
- cert_expires: Oct 15 06:48:32 2026 GMT
  host: api.spectrumoutage.us
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  9 08:27:32 2026 GMT
  host: spectrumoutage.us
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Spectrumoutage Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpectrumOutage API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SpectrumOutage API
provider_slug: spectrumoutage-api
slug: spectrumoutage-api-domain-security
source_filename: spectrumoutage-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.spectrumoutage.us\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 06:48:32 2026 GMT\n  hsts: false\n- host: spectrumoutage.us\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  9 08:27:32 2026 GMT\n  hsts: false\ndomains:\n- domain: spectrumoutage.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spectrumoutage-api/refs/heads/main/security/spectrumoutage-api-domain-security.yml
summary_line: TLSv1.2
tags:
- Spectrum
- outage
- Internet
- TV
- Phone
- Monitoring
- Status
- ZIP Code
- Telecom
- ISP
- network-status
- Crowdsourced
---
