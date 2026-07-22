---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: preteckt.com
  spf: true
hosts:
- cert_expires: Sep 21 03:31:13 2026 GMT
  host: preteckt.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Preteckt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Preteckt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Preteckt
provider_slug: preteckt
slug: preteckt-domain-security
source_filename: preteckt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: preteckt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:31:13 2026 GMT\n  hsts: false\ndomains:\n- domain: preteckt.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/preteckt/refs/heads/main/security/preteckt-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Predictive Maintenance
- Fleet Management
- Transportation
- Automotive
- Machine Learning
- Telematics
- IoT
---
