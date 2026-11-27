---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: referna.com
  spf: true
hosts:
- cert_expires: Feb  4 16:30:58 2027 GMT
  host: referna.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Referna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Referna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Referna
provider_slug: referna-com
slug: referna-com-domain-security
source_filename: referna-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: referna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 16:30:58 2027 GMT\n  hsts: false\ndomains:\n- domain: referna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/referna-com/security/referna-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Referral
- Tech
- IndependentExperts
- Networking
---
