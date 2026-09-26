---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aneirapharma.com
  spf: false
hosts:
- cert_expires: Dec 12 18:34:54 2026 GMT
  host: www.aneirapharma.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aneira Pharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aneira Pharma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Aneira Pharma
provider_slug: aneira-pharma
slug: aneira-pharma-domain-security
source_filename: aneira-pharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aneirapharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 18:34:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: aneirapharma.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aneira-pharma/refs/heads/main/security/aneira-pharma-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- HairGrowth
- Pharmaceuticals
- ClinicalTrials
---
