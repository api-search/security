---
api_specs:
- filename: biogen-developer-api-openapi.yml
  format: yaml
  label: Biogen Developer API
  slug: developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biogen/refs/heads/main/openapi/biogen-developer-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: biogen.com
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: developer.biogen.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: www.biogen.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Biogen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biogen, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Biogen
provider_slug: biogen
slug: biogen-domain-security
source_filename: biogen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.biogen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\n- host: www.biogen.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: biogen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biogen/refs/heads/main/security/biogen-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Biotechnology
- Healthcare
- Life Sciences
- Pharmaceuticals
- Neurology
- Fortune 500
---
