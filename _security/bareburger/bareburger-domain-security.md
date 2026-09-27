---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bareburger.com
  spf: false
hosts:
- cert_expires: Dec 26 03:43:09 2026 GMT
  host: bareburger.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bareburger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bareburger, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Bareburger
provider_slug: bareburger
slug: bareburger-domain-security
source_filename: bareburger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bareburger.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 03:43:09 2026 GMT\n  hsts: false\ndomains:\n- domain: bareburger.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bareburger/refs/heads/main/security/bareburger-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Restaurant
- Fast-casual
- Food
- Sustainability
---
