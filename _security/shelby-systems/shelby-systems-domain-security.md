---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shelbysystems.com
  spf: true
hosts:
- cert_expires: Jan 19 21:51:48 2027 GMT
  host: shelbysystems.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Shelby Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shelby Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Shelby Systems
provider_slug: shelby-systems
slug: shelby-systems-domain-security
source_filename: shelby-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shelbysystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 21:51:48 2027 GMT\n  hsts: false\ndomains:\n- domain: shelbysystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/shelby-systems/security/shelby-systems-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Church Management
- Church Accounting
- Online Giving
- Ministry Software
- Faith‑based Software
- Nonprofit Software
- Church Websites
- Background Checks
---
