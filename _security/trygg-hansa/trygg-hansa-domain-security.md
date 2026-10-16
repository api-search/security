---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: trygghansa.se
  spf: true
hosts:
- cert_expires: Nov 26 01:41:58 2026 GMT
  host: trygghansa.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trygg Hansa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trygg-Hansa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Trygg-Hansa
provider_slug: trygg-hansa
slug: trygg-hansa-domain-security
source_filename: trygg-hansa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trygghansa.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 01:41:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trygghansa.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trygg-hansa/refs/heads/main/security/trygg-hansa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Insurance
- Sweden
- Financial Services
- InsuranceTech
---
