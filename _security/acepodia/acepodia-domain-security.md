---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: acepodia.com
  spf: false
hosts:
- cert_expires: Oct 11 03:23:57 2026 GMT
  host: www.acepodia.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Acepodia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acepodia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Acepodia
provider_slug: acepodia
slug: acepodia-domain-security
source_filename: acepodia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acepodia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 11 03:23:57 2026 GMT\n  hsts: false\ndomains:\n- domain: acepodia.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acepodia/refs/heads/main/security/acepodia-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Biotechnology
- Cell Therapy
- Oncology
- Immunotherapy
- Life Sciences
- Clinical Stage
- Healthcare
---
