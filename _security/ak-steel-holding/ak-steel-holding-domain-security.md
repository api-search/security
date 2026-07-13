---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: clevelandcliffs.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aksteel.com
  spf: true
hosts:
- cert_expires: Sep 20 19:04:39 2026 GMT
  host: www.clevelandcliffs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: ir.aksteel.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ak Steel Holding Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AK Steel Holding, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AK Steel Holding
provider_slug: ak-steel-holding
slug: ak-steel-holding-domain-security
source_filename: ak-steel-holding-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clevelandcliffs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:04:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ir.aksteel.com\n  https: false\ndomains:\n- domain: clevelandcliffs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: aksteel.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ak-steel-holding/refs/heads/main/security/ak-steel-holding-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Automotive
- Manufacturing
- Materials
- Steel
- Metals
- Fortune 500
---
