---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: ETH Library Discovery API
  slug: discovery
  spec_type: OpenAPI
  url: https://eth-library.github.io/opendata-apis/
- filename: openapi.yaml
  format: yaml
  label: ETH Library ETHorama API
  slug: ethorama
  spec_type: OpenAPI
  url: https://eth-library.github.io/opendata-apis/
- filename: openapi.yaml
  format: yaml
  label: ETH Library Geo Information API
  slug: geo
  spec_type: OpenAPI
  url: https://eth-library.github.io/opendata-apis/
- filename: openapi.yaml
  format: yaml
  label: ETH Library Persons API
  slug: persons
  spec_type: OpenAPI
  url: https://eth-library.github.io/opendata-apis/
- filename: openapi.yaml
  format: yaml
  label: ETH Zurich Research Collection API
  slug: research-collection
  spec_type: OpenAPI
  url: https://eth-library.github.io/opendata-apis/
- filename: openapi.yaml
  format: yaml
  label: ETH Library Vector API
  slug: vector
  spec_type: OpenAPI
  url: https://eth-library.github.io/opendata-apis/
description: ''
domains:
- caa:
  - 0 iodef "mailto:id-bd-ws-pki-lra@id.ethz.ch"
  - 0 issuewild "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "quovadisglobal.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ethz.ch
  spf: true
hosts:
- cert_expires: Aug 23 23:59:59 2026 GMT
  host: ethz.ch
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 00:56:07 2026 GMT
  host: api.library.ethz.ch
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eth Zurich Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ETH Zurich – Swiss Federal Institute of Technology, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: ETH Zurich – Swiss Federal Institute of Technology
provider_slug: eth-zurich
slug: eth-zurich-domain-security
source_filename: eth-zurich-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ethz.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.library.ethz.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 00:56:07 2026 GMT\n  hsts: null\ndomains:\n- domain: ethz.ch\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:id-bd-ws-pki-lra@id.ethz.ch\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"quovadisglobal.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eth-zurich/refs/heads/main/security/eth-zurich-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Library
- Open Data
- Switzerland
---
