---
api_specs:
- filename: openssf-osv-openapi.yml
  format: yaml
  label: OSV (Open Source Vulnerabilities) API
  slug: osv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openssf/refs/heads/main/openapi/openssf-osv-openapi.yml
- filename: openssf-scorecard-openapi.yml
  format: yaml
  label: OpenSSF Scorecard API
  slug: scorecard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openssf/refs/heads/main/openapi/openssf-scorecard-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openssf.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: osv.dev
  spf: false
hosts:
- cert_expires: Sep 24 07:57:22 2026 GMT
  host: openssf.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 20:43:44 2026 GMT
  host: osv.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 14:00:19 2026 GMT
  host: api.osv.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openssf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenSSF, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenSSF
provider_slug: openssf
slug: openssf-domain-security
source_filename: openssf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openssf.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 07:57:22 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: osv.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:43:44 2026 GMT\n  hsts: false\n- host: api.osv.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:00:19 2026 GMT\n  hsts: null\ndomains:\n- domain: openssf.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: osv.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openssf/refs/heads/main/security/openssf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Linux Foundation
- Open Source
- Security
- Supply Chain
- Vulnerabilities
---
