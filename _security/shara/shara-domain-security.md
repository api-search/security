---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shara.co
  spf: true
hosts:
- cert_expires: Sep  7 14:40:09 2026 GMT
  host: shara.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shara Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shara, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shara
provider_slug: shara
slug: shara-domain-security
source_filename: shara-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shara.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 14:40:09 2026 GMT\n  hsts: false\ndomains:\n- domain: shara.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shara/refs/heads/main/security/shara-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Lending
- SME Finance
- Working Capital
- Financial Services
- Nigeria
- Loans
---
