---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: digitalremedy.com
  spf: true
hosts:
- cert_expires: Oct 13 04:47:02 2026 GMT
  host: www.digitalremedy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adready Cpxi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdReady (CPXi), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AdReady (CPXi)
provider_slug: adready-cpxi
slug: adready-cpxi-domain-security
source_filename: adready-cpxi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.digitalremedy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 04:47:02 2026 GMT\n  hsts: false\ndomains:\n- domain: digitalremedy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adready-cpxi/refs/heads/main/security/adready-cpxi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Commerce
- Advertising
- AdTech
- Marketing
- Programmatic
- Media
---
