---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flexspring.com
  spf: true
hosts:
- cert_expires: Dec  6 00:46:07 2026 GMT
  host: flexspring.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flexspring Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flexspring, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flexspring
provider_slug: flexspring
slug: flexspring-domain-security
source_filename: flexspring-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flexspring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 00:46:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flexspring.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/flexspring/security/flexspring-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR Integration
- Data Integration
- Enterprise Software
- Software-as-a-Service
- API Platform
---
