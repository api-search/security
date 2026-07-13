---
api_specs:
- filename: what3words-openapi.yml
  format: yaml
  label: what3words Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/what3words/refs/heads/main/openapi/what3words-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: what3words.com
  spf: true
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: what3words.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: developer.what3words.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: api.what3words.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: What3Words Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for what3words, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: what3words
provider_slug: what3words
slug: what3words-domain-security
source_filename: what3words-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: what3words.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\n- host: developer.what3words.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: false\n- host: api.what3words.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: what3words.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/what3words/refs/heads/main/security/what3words-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Geocoding
- Addressing
- Location
- Three Word Address
- Maps
---
