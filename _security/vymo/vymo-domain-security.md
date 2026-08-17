---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: vymo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getvymo.com
  spf: true
hosts:
- cert_expires: Oct 20 01:52:32 2026 GMT
  host: www.vymo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 01:52:32 2026 GMT
  host: vymo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 26 23:59:59 2027 GMT
  host: app.lms.getvymo.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vymo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vymo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Vymo
provider_slug: vymo
slug: vymo-domain-security
source_filename: vymo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vymo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 01:52:32 2026 GMT\n  hsts: false\n- host: vymo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 01:52:32 2026 GMT\n  hsts: false\n- host: app.lms.getvymo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: vymo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: getvymo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vymo/refs/heads/main/security/vymo-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Sales Tech
- Sales Engagement
- Financial Services
- Insurance
- Distribution Management
- CRM
- Collections
---
