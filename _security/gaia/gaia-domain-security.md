---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gaiafamily.com
  spf: false
hosts:
- cert_expires: Oct 10 04:25:06 2026 GMT
  host: www.gaiafamily.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gaia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gaia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Gaia
provider_slug: gaia
slug: gaia-domain-security
source_filename: gaia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gaiafamily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 04:25:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gaiafamily.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gaia/refs/heads/main/security/gaia-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthtech
- Fertility
- IVF
- Fintech
- Family Planning
- Reproductive Health
- Femtech
- Insurance
---
