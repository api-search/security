---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gametogen.com
  spf: true
hosts:
- cert_expires: Sep  6 16:39:15 2026 GMT
  host: www.gametogen.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gameto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gameto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Gameto
provider_slug: gameto
slug: gameto-domain-security
source_filename: gameto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gametogen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 16:39:15 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: gametogen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gameto/refs/heads/main/security/gameto-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotech Therapeutics
- Fertility
- Reproductive Health
- Women's Health
- IVF
- Stem Cells
---
