---
api_specs:
- filename: openlaws-openapi.yml
  format: yaml
  label: OpenLaws Legal Data API
  slug: openlaws
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlaws/refs/heads/main/openapi/openlaws-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openlaws.us
  spf: true
hosts:
- cert_expires: Sep 19 05:46:33 2026 GMT
  host: openlaws.us
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 23:24:17 2026 GMT
  host: api.openlaws.us
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openlaws Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenLaws, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenLaws
provider_slug: openlaws
slug: openlaws-domain-security
source_filename: openlaws-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openlaws.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 05:46:33 2026 GMT\n  hsts: false\n- host: api.openlaws.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 23:24:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openlaws.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openlaws/refs/heads/main/security/openlaws-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal
- Law
- Statutes
- Regulations
- Constitutions
- Case Law
- Citations
- Search
- RAG
- LegalTech
- RegTech
- Compliance
- GRC
- Government Data
---
