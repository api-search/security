---
api_specs:
- filename: smklog-com-openapi.yml
  format: yaml
  label: SMKlog Quote API
  slug: smklog-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smklog-com/refs/heads/main/openapi/smklog-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: smklog.com
  spf: true
hosts:
- cert_expires: Nov 20 02:45:24 2026 GMT
  host: smklog.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 21:27:59 2026 GMT
  host: quote-api.smklog.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Smklog Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SMKlog, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SMKlog
provider_slug: smklog-com
slug: smklog-com-domain-security
source_filename: smklog-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smklog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 02:45:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: quote-api.smklog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 21:27:59 2026 GMT\n  hsts: false\ndomains:\n- domain: smklog.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smklog-com/refs/heads/main/security/smklog-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Shipping
- Logistics
- Parcel Shipping
- shipping-rates
- Shipping Labels
- E-Commerce
- Agents
- MCP
- A2A
---
