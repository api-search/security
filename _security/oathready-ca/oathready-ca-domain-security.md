---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oathready.ca
  spf: true
hosts:
- cert_expires: Feb  8 17:47:39 2027 GMT
  host: oathready.ca
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oath Ready Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oath Ready, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Oath Ready
provider_slug: oathready-ca
slug: oathready-ca-domain-security
source_filename: oathready-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oathready.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 17:47:39 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oathready.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/oathready-ca/security/oathready-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Citizenship
- Free
- Practice
- Canada
---
