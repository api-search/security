---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: boem.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: marinecadastre.gov
  spf: true
hosts:
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: www.boem.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 06:57:28 2026 GMT
  host: marinecadastre.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 11:27:15 2026 GMT
  host: hub.marinecadastre.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bureau Of Ocean Energy Management Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bureau of Ocean Energy Management, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bureau of Ocean Energy Management
provider_slug: bureau-of-ocean-energy-management
slug: bureau-of-ocean-energy-management-domain-security
source_filename: bureau-of-ocean-energy-management-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boem.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: marinecadastre.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:57:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: hub.marinecadastre.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 11:27:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: boem.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: marinecadastre.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-ocean-energy-management/refs/heads/main/security/bureau-of-ocean-energy-management-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Federal Government
- Marine
- Oceans
- GIS
- Offshore
- Environmental
---
