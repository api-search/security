---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cloutdesk.com
  spf: true
hosts:
- cert_expires: Sep 29 02:42:18 2026 GMT
  host: cloutdesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloutjam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloutJam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CloutJam
provider_slug: cloutjam
slug: cloutjam-domain-security
source_filename: cloutjam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloutdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 02:42:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloutdesk.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloutjam/refs/heads/main/security/cloutjam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Influencer Marketing
- Creator Management
- Creator Economy
- Marketing
- Agentic AI
- Agents
---
