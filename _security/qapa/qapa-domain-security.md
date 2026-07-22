---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: qapa.fr
  spf: true
hosts:
- cert_expires: Oct  8 11:40:57 2026 GMT
  host: qapa.fr
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qapa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qapa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Qapa
provider_slug: qapa
slug: qapa-domain-security
source_filename: qapa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qapa.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 11:40:57 2026 GMT\n  hsts: null\ndomains:\n- domain: qapa.fr\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qapa/refs/heads/main/security/qapa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Recruitment
- Staffing
- Temporary Work
- Human Resources
- Jobs
- Marketplace
- France
---
