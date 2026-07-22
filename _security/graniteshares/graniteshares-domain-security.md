---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: graniteshares.com
  spf: true
hosts:
- cert_expires: Jan  8 16:15:28 2027 GMT
  host: graniteshares.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Graniteshares Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GraniteShares, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GraniteShares
provider_slug: graniteshares
slug: graniteshares-domain-security
source_filename: graniteshares-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: graniteshares.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 16:15:28 2027 GMT\n  hsts: false\ndomains:\n- domain: graniteshares.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graniteshares/refs/heads/main/security/graniteshares-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- ETF
- Asset Management
- Investments
- Leveraged ETFs
- Financial Services
---
