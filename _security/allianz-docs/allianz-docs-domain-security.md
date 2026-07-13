---
api_specs:
- filename: allianz-api-connect.yaml
  format: yaml
  label: Allianz API Connect
  slug: allianz-api-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/openapi/allianz-api-connect.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: allianz.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: allianz.com.au
  spf: true
hosts:
- cert_expires: Aug 12 16:58:20 2026 GMT
  host: www.allianz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 11:56:09 2026 GMT
  host: www.allianz.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 04:08:07 2026 GMT
  host: api.allianz.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Allianz Docs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allianz, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Allianz
provider_slug: allianz-docs
slug: allianz-docs-domain-security
source_filename: allianz-docs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.allianz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 16:58:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.allianz.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 11:56:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.allianz.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 04:08:07 2026 GMT\n  hsts: null\ndomains:\n- domain: allianz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: allianz.com.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/security/allianz-docs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Insurance
- Asset Management
---
