---
api_specs:
- filename: attentive-v1-openapi.yaml
  format: yaml
  label: Attentive API
  slug: attentive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-v1-openapi.yaml
- filename: attentive-v2-openapi.yaml
  format: yaml
  label: Attentive API V2
  slug: attentive-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-v2-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: attentive.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: attentivemobile.com
  spf: true
hosts:
- cert_expires: Oct 14 17:50:42 2026 GMT
  host: www.attentive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: api.attentivemobile.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Attentive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Attentive, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Attentive
provider_slug: attentive
slug: attentive-domain-security
source_filename: attentive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.attentive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 17:50:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.attentivemobile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: attentive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: attentivemobile.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/security/attentive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Martech
- SMS Marketing
- Email Marketing
- Ecommerce
- Marketing Automation
- Subscribers
- Webhooks
- Customer Engagement
---
