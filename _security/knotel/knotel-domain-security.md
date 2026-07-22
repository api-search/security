---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: knotel.com
  spf: true
hosts:
- cert_expires: Oct 10 20:25:58 2026 GMT
  host: knotel.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knotel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knotel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Knotel
provider_slug: knotel
slug: knotel-domain-security
source_filename: knotel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knotel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 20:25:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: knotel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knotel/refs/heads/main/security/knotel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Commercial Real Estate
- Flexible Workspace
- Managed Office
- Coworking
- Workplace Services
- PropTech
---
