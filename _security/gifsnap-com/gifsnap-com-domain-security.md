---
api_specs:
- filename: gifsnap-com-gifs-api-openapi.yml
  format: yaml
  label: Rowix Gifs API
  slug: gifsnap-com-gifs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gifsnap-com/openapi/gifsnap-com-gifs-api-openapi.yml
- filename: gifsnap-com-recommendations-api-openapi.yml
  format: yaml
  label: Rowix Recommendations API
  slug: gifsnap-com-recommendations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gifsnap-com/openapi/gifsnap-com-recommendations-api-openapi.yml
- filename: gifsnap-com-stickers-api-openapi.yml
  format: yaml
  label: Rowix Stickers API
  slug: gifsnap-com-stickers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gifsnap-com/openapi/gifsnap-com-stickers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gifsnap.com
  spf: true
hosts:
- cert_expires: Dec 17 23:03:26 2026 GMT
  host: gifsnap.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rowix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rowix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rowix
provider_slug: gifsnap-com
slug: gifsnap-com-domain-security
source_filename: gifsnap-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gifsnap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:03:26 2026 GMT\n  hsts: false\ndomains:\n- domain: gifsnap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gifsnap-com/security/gifsnap-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- GIF Search
- GIF Maker
- Mobile App
- Keyboard
---
