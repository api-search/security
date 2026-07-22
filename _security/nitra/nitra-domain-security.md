---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nitra.com
  spf: true
hosts:
- cert_expires: Sep 30 09:15:30 2026 GMT
  host: www.nitra.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nitra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nitra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Nitra
provider_slug: nitra
slug: nitra-domain-security
source_filename: nitra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nitra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 09:15:30 2026 GMT\n  hsts: false\ndomains:\n- domain: nitra.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nitra/refs/heads/main/security/nitra-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Healthcare
- Fintech
- Banking
- Payments
- Practice Management
- Spend Management
---
