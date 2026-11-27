---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: listsignal.com
  spf: true
hosts:
- cert_expires: Feb  7 02:52:31 2027 GMT
  host: listsignal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ListSignal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ListSignal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ListSignal
provider_slug: listsignal-com
slug: listsignal-com-domain-security
source_filename: listsignal-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: listsignal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 02:52:31 2027 GMT\n  hsts: false\ndomains:\n- domain: listsignal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/listsignal-com/security/listsignal-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Business Intelligence
- Data Analytics
- Software-as-a-Service
- E-Commerce
---
