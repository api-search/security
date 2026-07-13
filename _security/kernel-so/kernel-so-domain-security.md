---
api_specs:
- filename: kernel-openapi.yml
  format: yaml
  label: Kernel API
  slug: kernel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel-so/refs/heads/main/openapi/kernel-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kernel.sh
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: onkernel.com
  spf: true
hosts:
- cert_expires: Sep 21 13:04:32 2026 GMT
  host: www.kernel.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: api.onkernel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 07:36:14 2026 GMT
  host: mcp.onkernel.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kernel So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kernel, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kernel
provider_slug: kernel-so
slug: kernel-so-domain-security
source_filename: kernel-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kernel.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 13:04:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.onkernel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: null\n- host: mcp.onkernel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 07:36:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kernel.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: onkernel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kernel-so/refs/heads/main/security/kernel-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- AI
- Artificial Intelligence
- Browser Automation
- Browsers
- Computer Use
- Headless Browsers
- MCP
- Playwright
- Web Agents
---
