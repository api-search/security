---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ula.app
  spf: true
hosts:
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: ula.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ula Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ula, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ula
provider_slug: ula
slug: ula-domain-security
source_filename: ula-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ula.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ula.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ula/refs/heads/main/security/ula-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Marketplace
- B2B
- Commerce
- Retail
- Indonesia
- Defunct
---
