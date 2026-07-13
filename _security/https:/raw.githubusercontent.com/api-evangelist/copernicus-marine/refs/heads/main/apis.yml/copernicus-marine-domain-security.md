---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: copernicus.eu
  spf: true
hosts:
- cert_expires: Sep  1 12:27:00 2026 GMT
  host: marine.copernicus.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 06:51:58 2026 GMT
  host: toolbox-docs.marine.copernicus.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 00:17:13 2026 GMT
  host: data.marine.copernicus.eu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Copernicus Marine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Copernicus Marine, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Copernicus Marine
provider_slug: https://raw.githubusercontent.com/api-evangelist/copernicus-marine/refs/heads/main/apis.yml
slug: copernicus-marine-domain-security
source_filename: copernicus-marine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marine.copernicus.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 12:27:00 2026 GMT\n  hsts: false\n- host: toolbox-docs.marine.copernicus.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 06:51:58 2026 GMT\n  hsts: false\n- host: data.marine.copernicus.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:17:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: copernicus.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/https://raw.githubusercontent.com/api-evangelist/copernicus-marine/refs/heads/main/apis.yml/refs/heads/main/security/copernicus-marine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Ocean
- Marine
- Oceanography
- Sea Level
- Temperature
- Salinity
- Currents
- Biogeochemistry
- Climate
- Environment
- Satellite
- Forecast
- Reanalysis
- Open Data
- EU
---
