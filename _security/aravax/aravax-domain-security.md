---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aravax.com.au
  spf: true
hosts:
- cert_expires: Dec 15 06:57:33 2026 GMT
  host: www.aravax.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aravax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aravax, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aravax
provider_slug: aravax
slug: aravax-domain-security
source_filename: aravax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aravax.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 06:57:33 2026 GMT\n  hsts: false\ndomains:\n- domain: aravax.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aravax/refs/heads/main/security/aravax-domain-security.yml
summary_line: TLSv1.3
tags:
- Biotechnology
- Immunotherapy
- Food Allergy
- Clinical Trials
- Australia
---
