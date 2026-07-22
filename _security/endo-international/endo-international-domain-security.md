---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: endo.com
  spf: true
hosts:
- cert_expires: Dec 30 13:54:26 2026 GMT
  host: www.endo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Endo International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Endo International, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Endo International
provider_slug: endo-international
slug: endo-international-domain-security
source_filename: endo-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.endo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 13:54:26 2026 GMT\n  hsts: false\ndomains:\n- domain: endo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endo-international/refs/heads/main/security/endo-international-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Pharmaceuticals
- Specialty Pharma
- Generics
- Sterile Injectables
- Urology
- Orthopedics
- Chapter 11
- Opioid Settlement
---
