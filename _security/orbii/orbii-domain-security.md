---
api_specs:
- filename: orbii-uae-openapi-original.json
  format: json
  label: Orbii API (UAE)
  slug: orbii-api-uae
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-uae-openapi-original.json
- filename: orbii-ksa-openapi-original.json
  format: json
  label: Orbii KSA API
  slug: orbii-ksa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-ksa-openapi-original.json
- filename: orbii-omn-openapi-original.json
  format: json
  label: Orbii OMN API
  slug: orbii-omn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-omn-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orbii.ai
  spf: true
hosts:
- host: orbii.ai
  https: false
- cert_expires: Oct  4 17:53:09 2026 GMT
  host: api.docs.orbii.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:37:21 2026 GMT
  host: api.orbii.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orbii Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orbii, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Orbii
provider_slug: orbii
slug: orbii-domain-security
source_filename: orbii-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orbii.ai\n  https: false\n- host: api.docs.orbii.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 17:53:09 2026 GMT\n  hsts: false\n- host: api.orbii.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:37:21 2026 GMT\n  hsts: false\ndomains:\n- domain: orbii.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/security/orbii-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Ai
- Lending
- Credit
- Fintech
- Underwriting
- Banking
- SME
- Embedded Finance
- MENA
- Risk
---
