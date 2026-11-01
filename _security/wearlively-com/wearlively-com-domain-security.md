---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wearlively.com
  spf: true
hosts:
- cert_expires: Feb 10 07:07:36 2027 GMT
  host: www.wearlively.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wearlively Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lively, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lively
provider_slug: wearlively-com
slug: wearlively-com-domain-security
source_filename: wearlively-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wearlively.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 07:07:36 2027 GMT\n  hsts: null\ndomains:\n- domain: wearlively.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/wearlively-com/security/wearlively-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Wearables
- Platform
- API
- DataAnalytics
---
