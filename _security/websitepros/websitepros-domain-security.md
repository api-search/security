---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: web.com
  spf: true
hosts:
- cert_expires: Sep 28 21:46:28 2026 GMT
  host: www.web.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Websitepros Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WebsitePros, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WebsitePros
provider_slug: websitepros
slug: websitepros-domain-security
source_filename: websitepros-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.web.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 21:46:28 2026 GMT\n  hsts: null\ndomains:\n- domain: web.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/websitepros/refs/heads/main/security/websitepros-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Website Builder
- Web Hosting
- Domains
- Small Business
- Digital Marketing
- E-Commerce
---
