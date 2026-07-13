---
api_specs:
- filename: inttra-ocean-execution-openapi.yml
  format: yaml
  label: INTTRA Ocean Execution API
  slug: inttra-ocean-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/e2open/refs/heads/main/openapi/inttra-ocean-execution-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: e2open.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: inttra.com
  spf: true
hosts:
- cert_expires: Sep 17 10:23:38 2026 GMT
  host: www.e2open.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 05:33:58 2026 GMT
  host: apidocs.inttra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 21:07:38 2026 GMT
  host: api.e2open.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: E2Open Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for e2open, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: e2open
provider_slug: e2open
slug: e2open-domain-security
source_filename: e2open-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.e2open.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 10:23:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.inttra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 05:33:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.e2open.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 21:07:38 2026 GMT\n  hsts: null\ndomains:\n- domain: e2open.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: inttra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/e2open/refs/heads/main/security/e2open-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
