---
api_specs:
- filename: simplevoip-call-recordings-api-openapi.yml
  format: yaml
  label: SimpleVoIP Call Recordings API
  slug: simplevoip-call-recordings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simplevoip/openapi/simplevoip-call-recordings-api-openapi.yml
- filename: simplevoip-cdr-api-openapi.yml
  format: yaml
  label: SimpleVoIP CDR API
  slug: simplevoip-cdr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simplevoip/openapi/simplevoip-cdr-api-openapi.yml
- filename: simplevoip-music-on-hold-api-openapi.yml
  format: yaml
  label: SimpleVoIP Music on Hold API
  slug: simplevoip-music-on-hold-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simplevoip/openapi/simplevoip-music-on-hold-api-openapi.yml
- filename: simplevoip-sms-api-openapi.yml
  format: yaml
  label: SimpleVoIP SMS API
  slug: simplevoip-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simplevoip/openapi/simplevoip-sms-api-openapi.yml
- filename: simplevoip-time-of-day-api-openapi.yml
  format: yaml
  label: SimpleVoIP Time of Day API
  slug: simplevoip-time-of-day-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simplevoip/openapi/simplevoip-time-of-day-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: simplevoip.com
  spf: true
hosts:
- cert_expires: Mar 28 23:59:59 2027 GMT
  host: simplevoip.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Simplevoip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimpleVoIP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SimpleVoIP
provider_slug: simplevoip
slug: simplevoip-domain-security
source_filename: simplevoip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simplevoip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 28 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: simplevoip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/simplevoip/security/simplevoip-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- VoIP
- Communications
- UCaaS
- AI
- SMB
---
