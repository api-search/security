---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 409aproviders.com
  spf: true
hosts:
- cert_expires: Jan 10 12:40:35 2027 GMT
  host: 409aproviders.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 409A Providers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 409A Providers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 409A Providers
provider_slug: 409aproviders-com
slug: 409aproviders-com-domain-security
source_filename: 409aproviders-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 409aproviders.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 12:40:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 409aproviders.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/409aproviders-com/security/409aproviders-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
