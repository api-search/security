---
api_specs:
- filename: ontraport-openapi.yml
  format: yaml
  label: Ontraport REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontraport/refs/heads/main/openapi/ontraport-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ontraport.com
  spf: true
hosts:
- cert_expires: Sep  7 20:40:50 2026 GMT
  host: ontraport.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.ontraport.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ontraport Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ontraport, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ontraport
provider_slug: ontraport
slug: ontraport-domain-security
source_filename: ontraport-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ontraport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 20:40:50 2026 GMT\n  hsts: false\n- host: api.ontraport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: ontraport.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ontraport/refs/heads/main/security/ontraport-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CRM
- Marketing Automation
- Email Marketing
- Ecommerce
- Landing Pages
- Membership Sites
---
