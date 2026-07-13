---
api_specs:
- filename: openfigi-openapi.json
  format: json
  label: OpenFIGI API
  slug: openfigi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfigi/refs/heads/main/openapi/openfigi-openapi.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:reportvuln@bloomberg.net"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openfigi.com
  spf: true
hosts:
- cert_expires: Aug 31 23:59:59 2026 GMT
  host: www.openfigi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: api.openfigi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openfigi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenFIGI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenFIGI
provider_slug: openfigi
slug: openfigi-domain-security
source_filename: openfigi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openfigi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openfigi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: openfigi.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:reportvuln@bloomberg.net\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openfigi/refs/heads/main/security/openfigi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Instruments
---
