---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: connectedcannabisco.com
  spf: true
hosts:
- cert_expires: Jan  8 12:25:33 2027 GMT
  host: connectedcannabisco.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Connected Cannabis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connected Cannabis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Connected Cannabis
provider_slug: connected-cannabis
slug: connected-cannabis-domain-security
source_filename: connected-cannabis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: connectedcannabisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 12:25:33 2027 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: connectedcannabisco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connected-cannabis/refs/heads/main/security/connected-cannabis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cannabis
- Retail
- E-Commerce
- California
- Dispensary
---
