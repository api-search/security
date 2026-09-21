---
api_specs:
- filename: bmcxiv-com-openapi.yml
  format: yaml
  label: Breach402 API
  slug: breach402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmcxiv-com/refs/heads/main/openapi/bmcxiv-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bmcxiv.com
  spf: true
hosts:
- cert_expires: Oct 26 08:59:57 2026 GMT
  host: bmcxiv.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 08:59:57 2026 GMT
  host: breach402.bmcxiv.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Bmcxiv Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BMC XIV, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BMC XIV
provider_slug: bmcxiv-com
slug: bmcxiv-com-domain-security
source_filename: bmcxiv-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bmcxiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 08:59:57 2026 GMT\n  hsts: null\n- host: breach402.bmcxiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 08:59:57 2026 GMT\n  hsts: false\ndomains:\n- domain: bmcxiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bmcxiv-com/refs/heads/main/security/bmcxiv-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Cybersecurity
- Breach Intelligence
- Identity Protection
- Data Breaches
- Agents
- MCP
- A2A
- x402
---
