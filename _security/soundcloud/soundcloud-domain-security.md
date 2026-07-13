---
api_specs:
- filename: soundcloud-openapi.yml
  format: yaml
  label: SoundCloud API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcloud/refs/heads/main/openapi/soundcloud-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: soundcloud.com
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: soundcloud.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: developers.soundcloud.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: api.soundcloud.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Soundcloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SoundCloud, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SoundCloud
provider_slug: soundcloud
slug: soundcloud-domain-security
source_filename: soundcloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: soundcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.soundcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.soundcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: soundcloud.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundcloud/refs/heads/main/security/soundcloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Streaming
- Audio
- OAuth
- Tracks
- Playlists
---
