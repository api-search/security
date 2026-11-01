---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airbus.com
  spf: true
hosts:
- cert_expires: Dec  9 09:51:24 2026 GMT
  host: www.airbus.com
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Airbus Defence Space Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airbus Defence & Space, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Airbus Defence & Space
provider_slug: airbus-defence-space
slug: airbus-defence-space-domain-security
source_filename: airbus-defence-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airbus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 09:51:24 2026 GMT\n  hsts: true\n  hsts_max_age: 1000\ndomains:\n- domain: airbus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/airbus-defence-space/security/airbus-defence-space-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
