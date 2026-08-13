---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: elixiron.com
  spf: true
hosts:
- cert_expires: Oct 20 14:34:55 2026 GMT
  host: elixiron.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elixiron Immunotherapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elixiron Immunotherapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Elixiron Immunotherapeutics
provider_slug: elixiron-immunotherapeutics
slug: elixiron-immunotherapeutics-domain-security
source_filename: elixiron-immunotherapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elixiron.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 14:34:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: elixiron.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elixiron-immunotherapeutics/refs/heads/main/security/elixiron-immunotherapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Immunotherapy
- Life Sciences
- Clinical Trials
- Healthcare
- Taiwan
---
