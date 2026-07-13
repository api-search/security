---
api_specs:
- filename: cdisc-library-openapi.yml
  format: yaml
  label: CDISC Library API
  slug: cdisc-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-library-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cdisc.org
  spf: true
hosts:
- cert_expires: Sep 30 19:09:32 2026 GMT
  host: www.cdisc.org
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: library.cdisc.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cdisc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cdisc, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: cdisc
provider_slug: cdisc
slug: cdisc-domain-security
source_filename: cdisc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cdisc.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:09:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: library.cdisc.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cdisc.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/security/cdisc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
