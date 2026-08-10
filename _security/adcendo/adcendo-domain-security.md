---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adcendo.com
  spf: true
hosts:
- cert_expires: Oct 14 08:22:06 2026 GMT
  host: adcendo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adcendo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adcendo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adcendo
provider_slug: adcendo
slug: adcendo-domain-security
source_filename: adcendo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adcendo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 08:22:06 2026 GMT\n  hsts: false\ndomains:\n- domain: adcendo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adcendo/refs/heads/main/security/adcendo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Oncology
- Life Sciences
- Antibody-Drug Conjugates
- Clinical Stage
- Denmark
---
