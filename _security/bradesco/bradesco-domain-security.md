---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: banco.bradesco
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: banco.bradesco
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bradesco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bradesco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bradesco
provider_slug: bradesco
slug: bradesco-domain-security
source_filename: bradesco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: banco.bradesco\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: banco.bradesco\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bradesco/refs/heads/main/security/bradesco-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
