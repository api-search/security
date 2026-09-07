---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 4dlifetec.com
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: 4dlifetec.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 4Dlifetec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4D Lifetec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 4D Lifetec
provider_slug: 4dlifetec
slug: 4dlifetec-domain-security
source_filename: 4dlifetec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 4dlifetec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: 4dlifetec.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4dlifetec/refs/heads/main/security/4dlifetec-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Diagnostics
- Oncology
- Life Sciences
- Biotechnology
- Laboratory
- Medical Devices
- Switzerland
---
