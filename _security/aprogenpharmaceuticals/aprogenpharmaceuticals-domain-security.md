---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aprogen.com
  spf: true
hosts:
- cert_expires: Mar 21 23:59:59 2027 GMT
  host: www.aprogen.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aprogenpharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aprogenpharmaceuticals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aprogenpharmaceuticals
provider_slug: aprogenpharmaceuticals
slug: aprogenpharmaceuticals-domain-security
source_filename: aprogenpharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aprogen.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: aprogen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aprogenpharmaceuticals/refs/heads/main/security/aprogenpharmaceuticals-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Biopharma
- Antibodies
- Biotechnology
- Therapeutics
---
