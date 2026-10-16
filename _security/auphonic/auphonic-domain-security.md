---
api_specs:
- filename: auphonic-info-api-openapi.yml
  format: yaml
  label: Auphonic Info API
  slug: auphonic-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-info-api-openapi.yml
- filename: auphonic-presets-api-openapi.yml
  format: yaml
  label: Auphonic Presets API
  slug: auphonic-presets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-presets-api-openapi.yml
- filename: auphonic-productions-api-openapi.yml
  format: yaml
  label: Auphonic Productions API
  slug: auphonic-productions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-productions-api-openapi.yml
- filename: auphonic-services-api-openapi.yml
  format: yaml
  label: Auphonic Services API
  slug: auphonic-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-services-api-openapi.yml
- filename: auphonic-simple-api-api-openapi.yml
  format: yaml
  label: Auphonic Simple API
  slug: auphonic-simple-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-simple-api-api-openapi.yml
- filename: auphonic-user-api-openapi.yml
  format: yaml
  label: Auphonic User API
  slug: auphonic-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-user-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:admin@auphonic.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: auphonic.com
  spf: true
hosts:
- cert_expires: Dec  5 03:27:36 2026 GMT
  host: auphonic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Auphonic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auphonic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Auphonic
provider_slug: auphonic
slug: auphonic-domain-security
source_filename: auphonic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: auphonic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 03:27:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: auphonic.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:admin@auphonic.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/security/auphonic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Audio
- Podcasting
- AI
- Automation
- Media
---
