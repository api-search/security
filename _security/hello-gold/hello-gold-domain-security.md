---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hellogold.com
  spf: true
hosts:
- cert_expires: Sep  5 08:37:50 2026 GMT
  host: www.hellogold.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hello Gold Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hello Gold, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hello Gold
provider_slug: hello-gold
slug: hello-gold-domain-security
source_filename: hello-gold-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hellogold.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 08:37:50 2026 GMT\n  hsts: false\ndomains:\n- domain: hellogold.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hello-gold/refs/heads/main/security/hello-gold-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fintech
- Gold
- Savings
- Investing
- Islamic Finance
- Mobile App
- Malaysia
---
