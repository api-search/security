---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: staah.com
  spf: true
hosts:
- cert_expires: Feb  1 09:32:30 2027 GMT
  host: www.staah.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: STAAH Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for STAAH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: STAAH
provider_slug: staah
slug: staah-domain-security
source_filename: staah-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.staah.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 09:32:30 2027 GMT\n  hsts: null\ndomains:\n- domain: staah.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/staah/security/staah-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Hospitality
- Software-as-a-Service
- Channel Management
- Revenue Management
---
