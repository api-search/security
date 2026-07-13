---
api_specs:
- filename: manhattan-associates-omni-openapi.yml
  format: yaml
  label: Manhattan Active Omni and Enterprise Promise & Fulfill API
  slug: manhattan-active-omni-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manhattan-associates/refs/heads/main/openapi/manhattan-associates-omni-openapi.yml
- filename: manhattan-associates-wms-openapi.yml
  format: yaml
  label: Manhattan Active Supply Chain API
  slug: manhattan-active-supply-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manhattan-associates/refs/heads/main/openapi/manhattan-associates-wms-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: manh.com
  spf: true
hosts:
- cert_expires: Sep 27 05:03:27 2026 GMT
  host: developer.manh.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 07:59:19 2026 GMT
  host: www.manh.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 05:03:27 2026 GMT
  host: platform.developer.manh.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Manhattan Associates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for manhattan-associates, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: manhattan-associates
provider_slug: manhattan-associates
slug: manhattan-associates-domain-security
source_filename: manhattan-associates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.manh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 05:03:27 2026 GMT\n  hsts: false\n- host: www.manh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 07:59:19 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: platform.developer.manh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 05:03:27 2026 GMT\n  hsts: null\ndomains:\n- domain: manh.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manhattan-associates/refs/heads/main/security/manhattan-associates-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags: []
---
