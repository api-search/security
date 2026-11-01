---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: whistle.com
  spf: true
hosts:
- cert_expires: Apr 30 23:59:59 2027 GMT
  host: whistle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Whistle Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for whistle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: whistle
provider_slug: whistle-com
slug: whistle-com-domain-security
source_filename: whistle-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: whistle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: whistle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/whistle-com/security/whistle-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pet GPS
- Pet Health Monitoring
- Animal Tracking
- Pet Safety
---
