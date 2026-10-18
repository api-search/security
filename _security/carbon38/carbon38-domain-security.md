---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: carbon38.com
  spf: true
hosts:
- cert_expires: Jan  1 08:06:02 2027 GMT
  host: carbon38.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carbon38 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carbon38, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Carbon38
provider_slug: carbon38
slug: carbon38-domain-security
source_filename: carbon38-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carbon38.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 08:06:02 2027 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: carbon38.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbon38/refs/heads/main/security/carbon38-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fashion
- Activewear
- E-Commerce
- Apparel
---
