---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: pashouses.id
  spf: true
hosts:
- cert_expires: Oct  7 19:10:00 2026 GMT
  host: pashouses.id
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pashouses Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pashouses, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Pashouses
provider_slug: pashouses
slug: pashouses-domain-security
source_filename: pashouses-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pashouses.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 19:10:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pashouses.id\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pashouses/refs/heads/main/security/pashouses-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Proptech
- Real Estate
- Indonesia
- Marketplace
- Mortgage
- iBuyer
---
