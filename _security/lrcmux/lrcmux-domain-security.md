---
api_specs:
- filename: lrcmux-compatibility-api-openapi.yml
  format: yaml
  label: LRCMux Compatibility API
  slug: lrcmux-compatibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lrcmux/openapi/lrcmux-compatibility-api-openapi.yml
- filename: lrcmux-lyrics-api-openapi.yml
  format: yaml
  label: LRCMux Lyrics API
  slug: lrcmux-lyrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lrcmux/openapi/lrcmux-lyrics-api-openapi.yml
- filename: lrcmux-meta-api-openapi.yml
  format: yaml
  label: LRCMux Meta API
  slug: lrcmux-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lrcmux/openapi/lrcmux-meta-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lrcmux.dev
  spf: false
hosts:
- cert_expires: Dec  2 12:27:31 2026 GMT
  host: lrcmux.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lrcmux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LRCMux, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LRCMux
provider_slug: lrcmux
slug: lrcmux-domain-security
source_filename: lrcmux-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lrcmux.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 12:27:31 2026 GMT\n  hsts: false\ndomains:\n- domain: lrcmux.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lrcmux/security/lrcmux-domain-security.yml
summary_line: TLSv1.3
tags:
- Lyrics
- Music
- API
- Free
- NoAuth
---
