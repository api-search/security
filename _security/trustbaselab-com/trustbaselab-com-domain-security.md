---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: trustbaselab.com
  spf: false
hosts:
- cert_expires: Feb 12 15:01:53 2027 GMT
  host: trustbaselab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trustbase Lab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trustbase Lab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Trustbase Lab
provider_slug: trustbaselab-com
slug: trustbaselab-com-domain-security
source_filename: trustbaselab-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trustbaselab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 15:01:53 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trustbaselab.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/trustbaselab-com/security/trustbaselab-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Data
- Verification
- Industry
- API
- Platform
---
