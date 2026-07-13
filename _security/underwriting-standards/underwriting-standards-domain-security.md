---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: acord.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: limra.com
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: www.acord.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: www.limra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Underwriting Standards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Underwriting Standards, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Underwriting Standards
provider_slug: underwriting-standards
slug: underwriting-standards-domain-security
source_filename: underwriting-standards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acord.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\n- host: www.limra.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: acord.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: limra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/underwriting-standards/refs/heads/main/security/underwriting-standards-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Underwriting
- Insurance
- Standards
- ACORD
- Data Exchange
- InsurTech
---
