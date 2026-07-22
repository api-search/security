---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: neo.tax
  spf: true
hosts:
- cert_expires: Aug 26 01:53:43 2026 GMT
  host: neo.tax
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neotax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neo.Tax, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Neo.Tax
provider_slug: neotax
slug: neotax-domain-security
source_filename: neotax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neo.tax\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 01:53:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: neo.tax\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neotax/refs/heads/main/security/neotax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Tax
- R&D Tax Credit
- Accounting
- Fintech
- Compliance
- Artificial Intelligence
- Automation
---
