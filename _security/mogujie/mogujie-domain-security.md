---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mogujie.com
  spf: true
hosts:
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: mogujie.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mogujie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mogujie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: mogujie
provider_slug: mogujie
slug: mogujie-domain-security
source_filename: mogujie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mogujie.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mogujie.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mogujie/refs/heads/main/security/mogujie-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- E-Commerce
- Fashion
- Social Commerce
- Live Streaming
- Retail
- China
---
