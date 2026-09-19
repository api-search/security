---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agragene.com
  spf: true
hosts:
- cert_expires: Dec 10 11:47:20 2026 GMT
  host: www.agragene.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agragene Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agragene, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Agragene
provider_slug: agragene
slug: agragene-domain-security
source_filename: agragene-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agragene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 11:47:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: agragene.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agragene/refs/heads/main/security/agragene-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Agriculture
- AgTech
- Biotechnology
- Gene Editing
- Pest Control
- Sustainability
- Food and Beverage
- Life Sciences
- Company
---
