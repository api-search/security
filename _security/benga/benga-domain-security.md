---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: benga.eu
  spf: true
hosts:
- cert_expires: Nov 13 03:52:46 2026 GMT
  host: www.benga.eu
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Benga Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Benga, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Benga
provider_slug: benga
slug: benga-domain-security
source_filename: benga-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.benga.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 03:52:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: benga.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benga/refs/heads/main/security/benga-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Supplies
- Military Equipment
- Travel Products
- Custom Branding
- International
---
