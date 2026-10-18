---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: masabi.com
  spf: true
hosts:
- cert_expires: Jan  2 09:23:39 2027 GMT
  host: www.masabi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Masabi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Masabi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Masabi
provider_slug: masabi
slug: masabi-domain-security
source_filename: masabi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.masabi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 09:23:39 2027 GMT\n  hsts: false\ndomains:\n- domain: masabi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/masabi/refs/heads/main/security/masabi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Transit
- Software-as-a-Service
- MobileTicketing
- OpenPayments
---
