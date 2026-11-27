---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: fonixia.fr
  spf: true
hosts:
- cert_expires: Dec 15 16:42:06 2026 GMT
  host: fonixia.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fonixia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fonixia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Fonixia
provider_slug: fonixia-fr
slug: fonixia-fr-domain-security
source_filename: fonixia-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fonixia.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 16:42:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fonixia.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fonixia-fr/security/fonixia-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Artificial Intelligence
- Virtual Receptionist
- PhoneAutomation
- Small Business
---
