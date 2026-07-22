---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: armadin.com
  spf: true
hosts:
- cert_expires: Oct  4 04:31:27 2026 GMT
  host: www.armadin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Armadin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Armadin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Armadin
provider_slug: armadin
slug: armadin-domain-security
source_filename: armadin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.armadin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:31:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: armadin.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armadin/refs/heads/main/security/armadin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Cybersecurity
- Offensive Security
- Red Teaming
- Artificial Intelligence
- Agentic AI
- Penetration Testing
- Attack Surface Management
---
