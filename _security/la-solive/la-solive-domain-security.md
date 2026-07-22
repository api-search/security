---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: la-solive.com
  spf: true
hosts:
- cert_expires: Sep 12 13:15:55 2026 GMT
  host: www.la-solive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: La Solive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for La Solive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: La Solive
provider_slug: la-solive
slug: la-solive-domain-security
source_filename: la-solive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.la-solive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 13:15:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: la-solive.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/la-solive/refs/heads/main/security/la-solive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Climate
- Education
- Training
- Energy Efficiency
- Building Renovation
- Workforce Development
- France
- Sustainability
---
