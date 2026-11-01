---
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rallyup.com
  spf: true
hosts:
- cert_expires: Nov 28 19:15:03 2026 GMT
  host: rallyup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rallyup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rally Up, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rally Up
provider_slug: rallyup
slug: rallyup-domain-security
source_filename: rallyup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rallyup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 19:15:03 2026 GMT\n  hsts: false\ndomains:\n- domain: rallyup.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/rallyup/security/rallyup-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fundraising
- Nonprofit
- SaaS
- DigitalPlatform
---
