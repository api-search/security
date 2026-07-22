---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sidekickdata.io
  spf: true
hosts:
- cert_expires: Sep 24 23:32:02 2026 GMT
  host: sidekickdata.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sidekick Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sidekick Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Sidekick Data
provider_slug: sidekick-data
slug: sidekick-data-domain-security
source_filename: sidekick-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sidekickdata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:32:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sidekickdata.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sidekick-data/refs/heads/main/security/sidekick-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Real Estate
- Artificial Intelligence
- AI Assistant
- MLS
- Real Estate Agents
- SaaS
- Brokerage
---
