---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vinted.fr
  spf: true
hosts:
- cert_expires: Aug 29 07:02:10 2026 GMT
  host: www.vinted.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vinted Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vinted, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vinted
provider_slug: vinted
slug: vinted-domain-security
source_filename: vinted-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vinted.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 07:02:10 2026 GMT\n  hsts: false\ndomains:\n- domain: vinted.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vinted/refs/heads/main/security/vinted-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Marketplace
- Ecommerce
- Secondhand
- Fashion
- C2C
- Europe
---
