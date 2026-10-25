---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ailo.io
  spf: true
hosts:
- cert_expires: Jan  4 03:48:58 2027 GMT
  host: ailo.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ailo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ailo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ailo
provider_slug: ailo
slug: ailo-domain-security
source_filename: ailo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ailo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 03:48:58 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: ailo.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ailo/refs/heads/main/security/ailo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Property Management
- Real Estate
- PropTech
- Rent Payments
- Payments
- Australia
---
