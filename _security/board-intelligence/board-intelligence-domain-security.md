---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: boardintelligence.com
  spf: true
hosts:
- cert_expires: Nov 24 03:12:31 2026 GMT
  host: www.boardintelligence.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Board Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Board Intelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Board Intelligence
provider_slug: board-intelligence
slug: board-intelligence-domain-security
source_filename: board-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boardintelligence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 03:12:31 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\ndomains:\n- domain: boardintelligence.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/board-intelligence/refs/heads/main/security/board-intelligence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Board Management
- Governance
- Artificial Intelligence
- Board Reporting
- Entity Management
- Professional Services
- Financial Services
- Enterprise
---
