---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reposit.co.uk
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: reposit.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Reposit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reposit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Reposit
provider_slug: reposit
slug: reposit-domain-security
source_filename: reposit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reposit.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: reposit.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reposit/refs/heads/main/security/reposit-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Fintech
- PropTech
- Insurance
- Rental
- Deposits
- Real Estate
- United Kingdom
---
