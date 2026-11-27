---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: false
  domain: datafoodconsortium.org
  spf: true
hosts:
- cert_expires: Dec  6 13:43:48 2026 GMT
  host: datafoodconsortium.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Data Food Consortium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Data Food Consortium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Data Food Consortium
provider_slug: data-food-consortium
slug: data-food-consortium-domain-security
source_filename: data-food-consortium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datafoodconsortium.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 13:43:48 2026 GMT\n  hsts: false\ndomains:\n- domain: datafoodconsortium.org\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/data-food-consortium/security/data-food-consortium-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Food
- Open Standard
- Interoperability
- Non-Profit
---
