---
api_specs:
- filename: serpwow-openapi.yml
  format: yaml
  label: SerpWow
  slug: serpwow
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serpwow/refs/heads/main/openapi/serpwow-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trajectdata.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: serpwow.com
  spf: true
hosts:
- cert_expires: Sep 10 20:33:31 2026 GMT
  host: trajectdata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 21:17:55 2026 GMT
  host: api.serpwow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Serpwow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SerpWow, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SerpWow
provider_slug: serpwow
slug: serpwow-domain-security
source_filename: serpwow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trajectdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 20:33:31 2026 GMT\n  hsts: false\n- host: api.serpwow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 21:17:55 2026 GMT\n  hsts: null\ndomains:\n- domain: trajectdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: serpwow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serpwow/refs/heads/main/security/serpwow-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags: []
---
