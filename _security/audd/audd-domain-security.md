---
api_specs:
- filename: audd-openapi.yml
  format: yaml
  label: AudD Music Recognition API
  slug: music-recognition
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/openapi/audd-openapi.yml
- filename: audd-openapi.yml
  format: yaml
  label: AudD Recognize with Offset API
  slug: recognize-with-offset
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/openapi/audd-openapi.yml
- filename: audd-openapi.yml
  format: yaml
  label: AudD Humming Recognition API
  slug: humming-recognition
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/openapi/audd-openapi.yml
- filename: audd-openapi.yml
  format: yaml
  label: AudD Enterprise File Scan API
  slug: enterprise-file-scan
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/openapi/audd-openapi.yml
- filename: audd-openapi.yml
  format: yaml
  label: AudD Lyrics API
  slug: lyrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/openapi/audd-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: audd.io
  spf: true
hosts:
- cert_expires: Aug 16 03:38:57 2026 GMT
  host: audd.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 01:00:17 2026 GMT
  host: docs.audd.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 03:38:57 2026 GMT
  host: api.audd.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Audd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AudD, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AudD
provider_slug: audd
slug: audd-domain-security
source_filename: audd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audd.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 03:38:57 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.audd.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 01:00:17 2026 GMT\n  hsts: false\n- host: api.audd.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 03:38:57 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: audd.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/security/audd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Music
- Music Recognition
- Audio
- Fingerprinting
- Lyrics
---
