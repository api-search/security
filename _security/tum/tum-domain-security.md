---
api_specs:
- filename: tum-navigatum.yaml
  format: yaml
  label: NavigaTUM API
  slug: navigatum
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tum/refs/heads/main/openapi/tum-navigatum.yaml
- filename: tum-eat-api.yaml
  format: yaml
  label: eat-api (Mensa / Canteen API)
  slug: eat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tum/refs/heads/main/openapi/tum-eat-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tum.de
  spf: true
hosts:
- cert_expires: Oct 20 05:27:04 2026 GMT
  host: www.tum.de
  hsts: true
  hsts_max_age: 86400000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 16:16:55 2026 GMT
  host: nav.tum.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Technical University of Munich, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Technical University of Munich
provider_slug: tum
slug: tum-domain-security
source_filename: tum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tum.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 05:27:04 2026 GMT\n  hsts: true\n  hsts_max_age: 86400000\n- host: nav.tum.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 16:16:55 2026 GMT\n  hsts: false\ndomains:\n- domain: tum.de\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tum/refs/heads/main/security/tum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Germany
- Open Source
- Campus
- Open Data
---
