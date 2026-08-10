---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: conception.bio
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: www.conception.bio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conception Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conception, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Conception
provider_slug: conception
slug: conception-domain-security
source_filename: conception-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conception.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: conception.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conception/refs/heads/main/security/conception-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Reproductive Health
- Fertility
- In Vitro Gametogenesis
- Stem Cells
- Regenerative Medicine
- Life Sciences
- Tissue Engineering
- United States
---
