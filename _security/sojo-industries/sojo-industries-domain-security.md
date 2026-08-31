---
api_specs:
- filename: sojo-industries-victoria-agent-openapi.json
  format: json
  label: SOJO Planning Assistant (Victoria) API
  slug: sojo-planning-assistant-victoria-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sojo-industries/refs/heads/main/openapi/sojo-industries-victoria-agent-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sojoindustries.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: sojoshield.com
  spf: false
hosts:
- cert_expires: Oct 31 17:24:57 2026 GMT
  host: www.sojoindustries.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: sojoshield.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: victoria-agent.sojoshield.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sojo Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sojo Industries, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sojo Industries
provider_slug: sojo-industries
slug: sojo-industries-domain-security
source_filename: sojo-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sojoindustries.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 17:24:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sojoshield.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: false\n- host: victoria-agent.sojoshield.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sojoindustries.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: sojoshield.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sojo-industries/refs/heads/main/security/sojo-industries-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Supply Chain
- Traceability
- Food and Beverage
- Manufacturing
- Logistics
- Packaging
- Industrial Automation
- Blockchain
- Artificial Intelligence
- MCP
---
