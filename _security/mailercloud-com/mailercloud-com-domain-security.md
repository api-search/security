---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mailercloud.com
  spf: true
hosts:
- cert_expires: Jan  1 05:21:54 2027 GMT
  host: mailercloud.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mailercloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mailercloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Mailercloud
provider_slug: mailercloud-com
slug: mailercloud-com-domain-security
source_filename: mailercloud-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailercloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 05:21:54 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: mailercloud.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mailercloud-com/security/mailercloud-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email Marketing
- Software-as-a-Service
- Automation
- Marketing
---
