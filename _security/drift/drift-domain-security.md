---
api_specs:
- filename: drift-openapi.yml
  format: yaml
  label: Drift REST API
  slug: drift-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift/refs/heads/main/openapi/drift-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: drift.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: driftapi.com
  spf: false
hosts:
- cert_expires: Sep 26 20:17:29 2026 GMT
  host: www.drift.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 22:42:51 2026 GMT
  host: devdocs.drift.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: driftapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Drift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drift, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Drift
provider_slug: drift
slug: drift-domain-security
source_filename: drift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.drift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 20:17:29 2026 GMT\n  hsts: false\n- host: devdocs.drift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 22:42:51 2026 GMT\n  hsts: null\n- host: driftapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: drift.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: driftapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drift/refs/heads/main/security/drift-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Conversational Marketing
- Chatbots
- Sales
- Messaging
- Customer Engagement
---
