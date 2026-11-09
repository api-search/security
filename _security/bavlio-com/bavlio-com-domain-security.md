---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bavlio.com
  spf: true
hosts:
- cert_expires: Jan 19 16:53:42 2027 GMT
  host: bavlio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bavlio Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bavlio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bavlio
provider_slug: bavlio-com
slug: bavlio-com-domain-security
source_filename: bavlio-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bavlio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 16:53:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bavlio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bavlio-com/security/bavlio-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Sales
- Outreach
- Automation
- Lead Generation
- Company
---
