---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: conquestplanning.com
  spf: true
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: conquestplanning.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Conquestplanning Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conquestplanning, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Conquestplanning
provider_slug: conquestplanning
slug: conquestplanning-domain-security
source_filename: conquestplanning-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conquestplanning.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: conquestplanning.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conquestplanning/refs/heads/main/security/conquestplanning-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Financial-Planning
- AI
- Wealth-Management
- SaaS
---
