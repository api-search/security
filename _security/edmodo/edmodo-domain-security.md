---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: edmodo.com
  spf: true
hosts:
- cert_expires: Sep 21 14:17:22 2026 GMT
  host: edmodo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Edmodo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edmodo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Edmodo
provider_slug: edmodo
slug: edmodo-domain-security
source_filename: edmodo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edmodo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 14:17:22 2026 GMT\n  hsts: false\ndomains:\n- domain: edmodo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edmodo/refs/heads/main/security/edmodo-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Education
- EdTech
- Learning Management System
- Social Learning
- K-12
- Defunct
---
