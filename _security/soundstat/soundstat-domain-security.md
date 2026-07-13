---
api_specs:
- filename: soundstat-openapi.yml
  format: yaml
  label: SoundStat Track Analysis API
  slug: soundstat-track-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundstat/refs/heads/main/openapi/soundstat-openapi.yml
- filename: soundstat-openapi.yml
  format: yaml
  label: SoundStat Search & Discovery API
  slug: soundstat-search-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundstat/refs/heads/main/openapi/soundstat-openapi.yml
- filename: soundstat-openapi.yml
  format: yaml
  label: SoundStat Recommendations API
  slug: soundstat-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundstat/refs/heads/main/openapi/soundstat-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: soundstat.info
  spf: true
hosts:
- cert_expires: Aug  9 03:21:55 2026 GMT
  host: soundstat.info
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Soundstat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SoundStat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SoundStat
provider_slug: soundstat
slug: soundstat-domain-security
source_filename: soundstat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: soundstat.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 03:21:55 2026 GMT\n  hsts: false\ndomains:\n- domain: soundstat.info\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundstat/refs/heads/main/security/soundstat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Music
- Audio Analysis
- Audio Features
- Recommendations
- Track Analysis
- Spotify Alternative
---
