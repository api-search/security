---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: editasmedicine.com
  spf: true
hosts:
- cert_expires: Aug 24 16:16:45 2026 GMT
  host: editasmedicine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Editas Medicine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Editas Medicine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Editas Medicine
provider_slug: editas-medicine
slug: editas-medicine-domain-security
source_filename: editas-medicine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: editasmedicine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 16:16:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: editasmedicine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/editas-medicine/refs/heads/main/security/editas-medicine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Gene Editing
- CRISPR
- Genomics
- Therapeutics
- Pharmaceuticals
---
