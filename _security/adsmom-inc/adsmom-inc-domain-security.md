---
api_specs:
- filename: adsmom-inc-openapi.json
  format: json
  label: Adsmom REST API
  slug: adsmom-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adsmom-inc/refs/heads/main/openapi/adsmom-inc-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adsmom.com
  spf: true
hosts:
- cert_expires: Oct  2 08:10:53 2026 GMT
  host: adsmom.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 08:10:53 2026 GMT
  host: api.adsmom.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adsmom Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adsmom Inc., probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Adsmom Inc.
provider_slug: adsmom-inc
slug: adsmom-inc-domain-security
source_filename: adsmom-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adsmom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 08:10:53 2026 GMT\n  hsts: false\n- host: api.adsmom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 08:10:53 2026 GMT\n  hsts: null\ndomains:\n- domain: adsmom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adsmom-inc/refs/heads/main/security/adsmom-inc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advertising
- Ad Intelligence
- Competitive Intelligence
- Marketing
- Artificial Intelligence
- MCP
- Software-as-a-Service
- OpenAPI
- REST
- Analytics
- Social-Media
- agent-native
---
