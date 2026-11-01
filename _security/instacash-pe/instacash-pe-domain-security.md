---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: instacash.pe
  spf: true
hosts:
- cert_expires: Mar 26 23:59:59 2027 GMT
  host: instacash.pe
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Instacash Pe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PreAuth (Instacash), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PreAuth (Instacash)
provider_slug: instacash-pe
slug: instacash-pe-domain-security
source_filename: instacash-pe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: instacash.pe\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: instacash.pe\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/instacash-pe/security/instacash-pe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
