---
api_specs:
- filename: djamo-webhooks-asyncapi.yml
  format: yaml
  label: Djamo Business API
  slug: djamo-business-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/djamo/refs/heads/main/asyncapi/djamo-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: djamo.com
  spf: true
hosts:
- cert_expires: Sep 14 19:30:25 2026 GMT
  host: www.djamo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Djamo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Djamo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Djamo
provider_slug: djamo
slug: djamo-domain-security
source_filename: djamo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.djamo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:30:25 2026 GMT\n  hsts: false\ndomains:\n- domain: djamo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/djamo/refs/heads/main/security/djamo-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Financial Services
- Fintech
- Payments
- Banking
- Money Transfer
- Africa
- Côte d'Ivoire
- Sénégal
---
