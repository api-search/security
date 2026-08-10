---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: slingshotbio.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: myshopify.com
  spf: true
hosts:
- cert_expires: Sep 24 05:28:28 2026 GMT
  host: www.slingshotbio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 15:01:35 2026 GMT
  host: slingshot-bio.myshopify.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: 9l0m1rv5.api.sanity.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Slingshot Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Slingshot Biosciences, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Slingshot Biosciences
provider_slug: slingshot-biosciences
slug: slingshot-biosciences-domain-security
source_filename: slingshot-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.slingshotbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 05:28:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: slingshot-bio.myshopify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 15:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: 9l0m1rv5.api.sanity.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: slingshotbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: myshopify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slingshot-biosciences/refs/heads/main/security/slingshot-biosciences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Flow Cytometry
- Laboratory
- Synthetic Biology
- Diagnostics
- Cell Therapy
- E-Commerce
- GraphQL
- MCP
---
