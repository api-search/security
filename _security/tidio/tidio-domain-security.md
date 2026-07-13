---
api_specs:
- filename: tidio-openapi-openapi.yml
  format: yaml
  label: Tidio OpenAPI (REST)
  slug: tidio-openapi-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidio/refs/heads/main/openapi/tidio-openapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tidio.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tidio.co
  spf: false
hosts:
- cert_expires: Sep 13 03:22:56 2026 GMT
  host: www.tidio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 05:27:00 2026 GMT
  host: developers.tidio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: api.tidio.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tidio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tidio, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tidio
provider_slug: tidio
slug: tidio-domain-security
source_filename: tidio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tidio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 03:22:56 2026 GMT\n  hsts: false\n- host: developers.tidio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 05:27:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tidio.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: tidio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tidio.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tidio/refs/heads/main/security/tidio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- live chat
- chatbot
- customer service
- AI
- help desk
- ticketing
- conversations
- contacts
- webhooks
- widget
---
