---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aible.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: iamaible.com
  spf: true
hosts:
- cert_expires: Nov 18 00:45:10 2026 GMT
  host: www.aible.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: api.iamaible.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Aible Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aible, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aible
provider_slug: aible
slug: aible-domain-security
source_filename: aible-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aible.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 00:45:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.iamaible.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aible.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: iamaible.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aible/refs/heads/main/security/aible-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Machine-Learning
- AutoML
- Analytics
- Data Science
- AI Agents
- Generative AI
- Enterprise Software
- Cloud
- Company
---
