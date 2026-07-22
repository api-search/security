---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: innoventbio.com
  spf: true
hosts:
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: innoventbio.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Innovent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Innovent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Innovent
provider_slug: innovent
slug: innovent-domain-security
source_filename: innovent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: innoventbio.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: innoventbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innovent/refs/heads/main/security/innovent-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Healthcare
- Biotechnology
- Pharmaceuticals
- Biologics
- Oncology
- Life Sciences
---
