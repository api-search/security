---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sonomabio.com
  spf: true
hosts:
- cert_expires: Oct  2 13:16:26 2026 GMT
  host: sonomabio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sonoma Biotherapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sonoma Biotherapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sonoma Biotherapeutics
provider_slug: sonoma-biotherapeutics
slug: sonoma-biotherapeutics-domain-security
source_filename: sonoma-biotherapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sonomabio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:16:26 2026 GMT\n  hsts: false\ndomains:\n- domain: sonomabio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonoma-biotherapeutics/refs/heads/main/security/sonoma-biotherapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotech
- Cell Therapy
- Immunology
- Autoimmune
- Biopharmaceutical
- Regulatory T Cells
---
