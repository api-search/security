---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: defisolutions.com
  spf: true
hosts:
- cert_expires: Oct  3 15:11:49 2026 GMT
  host: defisolutions.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Defi Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for defi SOLUTIONS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: defi SOLUTIONS
provider_slug: defi-solutions
slug: defi-solutions-domain-security
source_filename: defi-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: defisolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:11:49 2026 GMT\n  hsts: false\ndomains:\n- domain: defisolutions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defi-solutions/refs/heads/main/security/defi-solutions-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Lending
- Loan Origination
- Loan Servicing
- Auto Finance
- Financial Services
- SaaS
---
