---
api_specs:
- filename: timoni-openapi.yml
  format: yaml
  label: Timoni Module Registry API
  slug: timoni
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timoni/refs/heads/main/openapi/timoni-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: timoni.sh
  spf: false
- caa:
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "sectigo.com"
  dmarc: false
  dnssec: false
  domain: ghcr.io
  spf: false
hosts:
- cert_expires: Aug 24 08:28:05 2026 GMT
  host: timoni.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: ghcr.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Timoni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Timoni, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Timoni
provider_slug: timoni
slug: timoni-domain-security
source_filename: timoni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: timoni.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:28:05 2026 GMT\n  hsts: false\n- host: ghcr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: timoni.sh\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: ghcr.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timoni/refs/heads/main/security/timoni-domain-security.yml
summary_line: TLSv1.3
tags:
- Containers
- Kubernetes
- Package Manager
- CUE
---
