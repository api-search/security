---
api_specs:
- filename: luxury-presence-cms-openapi.json
  format: json
  label: Luxury Presence Public API
  slug: luxury-presence-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luxury-presence/refs/heads/main/openapi/luxury-presence-cms-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: luxurypresence.com
  spf: true
hosts:
- cert_expires: Sep 22 16:28:48 2026 GMT
  host: www.luxurypresence.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: api.luxurypresence.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Luxury Presence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Luxury Presence, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Luxury Presence
provider_slug: luxury-presence
slug: luxury-presence-domain-security
source_filename: luxury-presence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.luxurypresence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 16:28:48 2026 GMT\n  hsts: false\n- host: api.luxurypresence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: luxurypresence.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luxury-presence/refs/heads/main/security/luxury-presence-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Vertical Software
- Real Estate
- PropTech
- CRM
- Marketing
- Websites
- Webhooks
- Lead Generation
---
