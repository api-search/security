---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: usfoods.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cleo.com
  spf: true
hosts:
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: www.usfoods.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 07:20:16 2026 GMT
  host: www.cleo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Foods, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: US Foods
provider_slug: us-foods
slug: us-foods-domain-security
source_filename: us-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usfoods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: www.cleo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 07:20:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usfoods.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cleo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-foods/refs/heads/main/security/us-foods-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food Service
- Fortune 500
- Distribution
- Supply Chain
- eCommerce
---
