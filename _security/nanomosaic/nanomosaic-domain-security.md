---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nanomosaicllc.com
  spf: true
hosts:
- cert_expires: Oct  1 03:33:15 2026 GMT
  host: www.nanomosaicllc.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nanomosaic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NanoMosaic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NanoMosaic
provider_slug: nanomosaic
slug: nanomosaic-domain-security
source_filename: nanomosaic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nanomosaicllc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:33:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nanomosaicllc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nanomosaic/refs/heads/main/security/nanomosaic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotech Therapeutics
- Proteomics
- Multiomics
- Gene Therapy
- Neurology
- Life Sciences
---
