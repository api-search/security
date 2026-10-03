---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azumo.com
  spf: true
hosts:
- cert_expires: Dec 13 01:46:56 2026 GMT
  host: azumo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Azumo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azumo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azumo
provider_slug: azumo
slug: azumo-domain-security
source_filename: azumo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: azumo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 01:46:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azumo.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azumo/refs/heads/main/security/azumo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Software Development
- Artificial Intelligence
- Custom Solutions
- Cloud Services
---
