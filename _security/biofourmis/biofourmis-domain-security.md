---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: biofourmis.com
  spf: true
hosts:
- cert_expires: Oct 28 14:44:32 2026 GMT
  host: biofourmis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Biofourmis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biofourmis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Biofourmis
provider_slug: biofourmis
slug: biofourmis-domain-security
source_filename: biofourmis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biofourmis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 14:44:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: biofourmis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biofourmis/refs/heads/main/security/biofourmis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Remote Patient Monitoring
- Hospital at Home
- Care Delivery
- Life Sciences
- Health Technology
- Wearables
---
