---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: agrevolution.in
  spf: true
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: agrevolution.in
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dehaat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeHaat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DeHaat
provider_slug: dehaat
slug: dehaat-domain-security
source_filename: dehaat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agrevolution.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: agrevolution.in\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dehaat/refs/heads/main/security/dehaat-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Agtech
- Agriculture
- Marketplace
- Rural
- Supply Chain
- India
- AI
---
