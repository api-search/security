---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: primemedicine.com
  spf: true
hosts:
- cert_expires: Aug 30 17:31:33 2026 GMT
  host: primemedicine.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prime Medicine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prime Medicine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Prime Medicine
provider_slug: prime-medicine
slug: prime-medicine-domain-security
source_filename: prime-medicine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: primemedicine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 17:31:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: primemedicine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prime-medicine/refs/heads/main/security/prime-medicine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Gene Editing
- Prime Editing
- Genetic Medicine
- Therapeutics
---
