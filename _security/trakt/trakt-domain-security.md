---
api_specs:
- filename: trakt-openapi.yml
  format: yaml
  label: Trakt API v2
  slug: trakt-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakt/refs/heads/main/openapi/trakt-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: trakt.tv
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apiary.io
  spf: true
hosts:
- cert_expires: Oct  9 13:44:49 2026 GMT
  host: trakt.tv
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: trakt.docs.apiary.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:44:49 2026 GMT
  host: api.trakt.tv
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trakt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trakt, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Trakt
provider_slug: trakt
slug: trakt-domain-security
source_filename: trakt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trakt.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:44:49 2026 GMT\n  hsts: false\n- host: trakt.docs.apiary.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: false\n- host: api.trakt.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:44:49 2026 GMT\n  hsts: null\ndomains:\n- domain: trakt.tv\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: apiary.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trakt/refs/heads/main/security/trakt-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Video
- Movies
- Television
- Media Tracking
- Scrobble
- Recommendations
- Social
- OAuth2
- Public APIs
---
