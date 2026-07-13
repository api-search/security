---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: energy.gov
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.energy.gov
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Office Of Fossil Energy And Carbon Management Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Office of Fossil Energy and Carbon Management, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Office of Fossil Energy and Carbon Management
provider_slug: office-of-fossil-energy-and-carbon-management
slug: office-of-fossil-energy-and-carbon-management-domain-security
source_filename: office-of-fossil-energy-and-carbon-management-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.energy.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: energy.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/office-of-fossil-energy-and-carbon-management/refs/heads/main/security/office-of-fossil-energy-and-carbon-management-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
---
