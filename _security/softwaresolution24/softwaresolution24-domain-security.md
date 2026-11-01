---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: softwaresolution24.com
  spf: true
hosts:
- cert_expires: Dec 25 01:38:04 2026 GMT
  host: softwaresolution24.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Softwaresolution24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Software Solution 24, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Software Solution 24
provider_slug: softwaresolution24
slug: softwaresolution24-domain-security
source_filename: softwaresolution24-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: softwaresolution24.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 01:38:04 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: softwaresolution24.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/softwaresolution24/security/softwaresolution24-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Software
- Retail
- Microsoft
- Licensing
- E-Commerce
---
