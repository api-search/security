---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kasahorow.com
  spf: true
hosts:
- cert_expires: Feb  9 17:04:06 2027 GMT
  host: kasahorow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: kasahorow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for kasahorow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: kasahorow
provider_slug: kasahorow-com
slug: kasahorow-com-domain-security
source_filename: kasahorow-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kasahorow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 17:04:06 2027 GMT\n  hsts: false\ndomains:\n- domain: kasahorow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kasahorow-com/security/kasahorow-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Language
- Education
- Community
- Platform
- Multilingual
---
