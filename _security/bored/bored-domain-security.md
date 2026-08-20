---
api_specs:
- filename: bored-activities-api-openapi.yml
  format: yaml
  label: Bored API Activities API
  slug: bored-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bored/refs/heads/main/openapi/bored-activities-api-openapi.yml
- filename: bored-facts-api-openapi.yml
  format: yaml
  label: Bored API Facts API
  slug: bored-facts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bored/refs/heads/main/openapi/bored-facts-api-openapi.yml
- filename: bored-riddles-api-openapi.yml
  format: yaml
  label: Bored API Riddles API
  slug: bored-riddles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bored/refs/heads/main/openapi/bored-riddles-api-openapi.yml
- filename: bored-suggestions-api-openapi.yml
  format: yaml
  label: Bored API Suggestions API
  slug: bored-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bored/refs/heads/main/openapi/bored-suggestions-api-openapi.yml
- filename: bored-websites-api-openapi.yml
  format: yaml
  label: Bored API Websites API
  slug: bored-websites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bored/refs/heads/main/openapi/bored-websites-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: boredapi.com
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: appbrewery.com
  spf: true
hosts:
- host: www.boredapi.com
  https: false
- cert_expires: Aug 21 02:59:42 2026 GMT
  host: bored-api.appbrewery.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bored Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bored API, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Bored API
provider_slug: bored
slug: bored-domain-security
source_filename: bored-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boredapi.com\n  https: false\n- host: bored-api.appbrewery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 02:59:42 2026 GMT\n  hsts: false\ndomains:\n- domain: boredapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: appbrewery.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bored/refs/heads/main/security/bored-domain-security.yml
summary_line: TLSv1.3
tags:
- Activities
- Boredom
- Community
- Development
- Discovery
- Education
- Facts
- Free
- MEVN
- No Auth
- Open-Source
- Public APIs
- Recreation
- Riddles
- Suggestions
- Websites
---
