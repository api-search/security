---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bond.bio
  spf: true
hosts:
- cert_expires: Dec 13 00:51:47 2026 GMT
  host: bond.bio
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bond Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bond Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bond Biosciences
provider_slug: bond-biosciences
slug: bond-biosciences-domain-security
source_filename: bond-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bond.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 00:51:47 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: bond.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bond-biosciences/refs/heads/main/security/bond-biosciences-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biopharma
- Therapeutics
- Ion‑related diseases
- Clinical Stage
---
