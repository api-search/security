---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deepinstinct.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deepinstinctweb.com
  spf: false
hosts:
- cert_expires: Sep  5 14:23:53 2026 GMT
  host: www.deepinstinct.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 19:26:11 2026 GMT
  host: portal.deepinstinct.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: your-tenant.customers.deepinstinctweb.com
  https: false
kind: domain-security
layout: security
method: probed
name: Deep Instinct Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deep Instinct, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Deep Instinct
provider_slug: deep-instinct
slug: deep-instinct-domain-security
source_filename: deep-instinct-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deepinstinct.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 14:23:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.deepinstinct.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 19:26:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: your-tenant.customers.deepinstinctweb.com\n  https: false\ndomains:\n- domain: deepinstinct.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: deepinstinctweb.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deep-instinct/refs/heads/main/security/deep-instinct-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cybersecurity
- endpoint-security
- malware-prevention
- ransomware
- deep-learning
- threat-prevention
- data-security
- edr
- soc-automation
- MCP
---
