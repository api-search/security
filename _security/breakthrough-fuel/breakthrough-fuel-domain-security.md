---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: breakthroughfuel.com
  spf: true
hosts:
- cert_expires: Jan 20 18:35:31 2027 GMT
  host: breakthroughfuel.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Breakthrough Fuel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Breakthrough Fuel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Breakthrough Fuel
provider_slug: breakthrough-fuel
slug: breakthrough-fuel-domain-security
source_filename: breakthrough-fuel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: breakthroughfuel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 18:35:31 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: breakthroughfuel.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/breakthrough-fuel/security/breakthrough-fuel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Transportation
- Fuel Management
- Logistics
- Sustainability
---
