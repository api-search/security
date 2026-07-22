---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: novaintelligence.com
  spf: true
hosts:
- cert_expires: Oct  4 14:30:36 2026 GMT
  host: www.novaintelligence.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nova Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nova, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nova
provider_slug: nova
slug: nova-domain-security
source_filename: nova-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.novaintelligence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:30:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: novaintelligence.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nova/refs/heads/main/security/nova-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- SAP
- Agentic AI
- Enterprise Software
- Developer Productivity
- Code Intelligence
---
