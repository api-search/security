---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 123elec.com
  spf: true
hosts:
- cert_expires: Dec 24 12:06:34 2026 GMT
  host: 123elec.com
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 123Elec Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 123elec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 123elec
provider_slug: 123elec-com
slug: 123elec-com-domain-security
source_filename: 123elec-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 123elec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 12:06:34 2026 GMT\n  hsts: true\n  hsts_max_age: 16000000\ndomains:\n- domain: 123elec.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/123elec-com/security/123elec-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Electrical
- Hardware
- Retail
- France
---
