---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mintsoft.co.uk
  spf: true
hosts:
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: mintsoft.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mintsoft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mintsoft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mintsoft
provider_slug: mintsoft
slug: mintsoft-domain-security
source_filename: mintsoft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mintsoft.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mintsoft.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mintsoft/security/mintsoft-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Warehouse
- Logistics
- SaaS
- E-commerce
- Fulfilment
- Company
---
