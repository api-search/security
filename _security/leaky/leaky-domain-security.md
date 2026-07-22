---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: leaky.com
  spf: true
hosts:
- cert_expires: Oct  6 19:10:55 2026 GMT
  host: leaky.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leaky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leaky, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Leaky
provider_slug: leaky
slug: leaky-domain-security
source_filename: leaky-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leaky.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:10:55 2026 GMT\n  hsts: false\ndomains:\n- domain: leaky.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaky/refs/heads/main/security/leaky-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Insurance
- InsurTech
- Auto Insurance
- Insurance Comparison
- Price Comparison
- Consumer Finance
- Defunct
---
