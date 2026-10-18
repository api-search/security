---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cwsisecurity.com
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: cwsisecurity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cwsi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CWSI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CWSI
provider_slug: cwsi
slug: cwsi-domain-security
source_filename: cwsi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cwsisecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cwsisecurity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cwsi/refs/heads/main/security/cwsi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Compliance
- Cybersecurity
- Enterprise
- United Kingdom
---
