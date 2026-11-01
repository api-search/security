---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: redsys.es
  spf: true
hosts:
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: redsys.es
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Redsys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redsys, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Redsys
provider_slug: redsys
slug: redsys-domain-security
source_filename: redsys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: redsys.es\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: redsys.es\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/redsys/security/redsys-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Payments
- Financial Services
- Acquiring
- Issuing
---
