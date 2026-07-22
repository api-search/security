---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: azos.com.br
  spf: true
hosts:
- cert_expires: Oct  2 23:58:31 2026 GMT
  host: azos.com.br
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Azos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Azos
provider_slug: azos
slug: azos-domain-security
source_filename: azos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: azos.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:58:31 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: azos.com.br\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azos/refs/heads/main/security/azos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Insurance
- Insurtech
- Life Insurance
- Brazil
- Financial Services
- Digital Insurance
---
