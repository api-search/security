---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gravity.com
  spf: true
hosts:
- cert_expires: Jan 26 18:06:14 2027 GMT
  host: www.gravity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gravity Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gravity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gravity
provider_slug: gravity-com
slug: gravity-com-domain-security
source_filename: gravity-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gravity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 18:06:14 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gravity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gravity-com/security/gravity-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- WordPress
- Forms
- Automation
- Marketplace
---
