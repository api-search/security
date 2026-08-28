---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: revagenix.com
  spf: true
hosts:
- cert_expires: Sep 30 11:40:26 2026 GMT
  host: www.revagenix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revagenix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revagenix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Revagenix
provider_slug: revagenix
slug: revagenix-domain-security
source_filename: revagenix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.revagenix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 11:40:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: revagenix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revagenix/refs/heads/main/security/revagenix-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Therapeutics
- Anti-Infectives
- Respiratory
- Clinical Stage
- Drug Discovery
- Private Company
---
