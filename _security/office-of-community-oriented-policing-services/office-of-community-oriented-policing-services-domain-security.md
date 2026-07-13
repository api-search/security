---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usdoj.gov
  spf: true
hosts:
- cert_expires: Sep 16 20:44:39 2026 GMT
  host: cops.usdoj.gov
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Office Of Community Oriented Policing Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Office of Community Oriented Policing Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Office of Community Oriented Policing Services
provider_slug: office-of-community-oriented-policing-services
slug: office-of-community-oriented-policing-services-domain-security
source_filename: office-of-community-oriented-policing-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cops.usdoj.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 20:44:39 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: usdoj.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/office-of-community-oriented-policing-services/refs/heads/main/security/office-of-community-oriented-policing-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
---
