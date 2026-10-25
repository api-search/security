---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: evt.com
  spf: true
hosts:
- cert_expires: Dec 10 09:01:32 2026 GMT
  host: evt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Evt Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EVT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EVT
provider_slug: evt-com
slug: evt-com-domain-security
source_filename: evt-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 09:01:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: evt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evt-com/refs/heads/main/security/evt-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Entertainment
- Cinemas
- Hospitality
- Hotels
- Travel
- Leisure
- Australia
---
