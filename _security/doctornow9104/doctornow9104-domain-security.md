---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: docnow.ai
  spf: true
hosts:
- cert_expires: Jan  9 10:14:49 2027 GMT
  host: docnow.ai
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Doctornow9104 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Doctornow9104, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Doctornow9104
provider_slug: doctornow9104
slug: doctornow9104-domain-security
source_filename: doctornow9104-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docnow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 10:14:49 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: docnow.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/doctornow9104/security/doctornow9104-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
