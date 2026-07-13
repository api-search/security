---
api_specs:
- filename: partnerstack-openapi.yml
  format: yaml
  label: PartnerStack
  slug: partnerstack
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/partnerstack/refs/heads/main/openapi/partnerstack-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: partnerstack.com
  spf: true
hosts:
- cert_expires: Aug 17 04:48:50 2026 GMT
  host: partnerstack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 17:00:47 2026 GMT
  host: docs.partnerstack.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 03:28:28 2026 GMT
  host: api.partnerstack.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Partnerstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PartnerStack, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PartnerStack
provider_slug: partnerstack
slug: partnerstack-domain-security
source_filename: partnerstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: partnerstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 04:48:50 2026 GMT\n  hsts: false\n- host: docs.partnerstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:00:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.partnerstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 03:28:28 2026 GMT\n  hsts: null\ndomains:\n- domain: partnerstack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/partnerstack/refs/heads/main/security/partnerstack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Partnerships
- Affiliate
- SaaS
---
