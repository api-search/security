---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: withshepherd.com
  spf: true
hosts:
- cert_expires: Nov 25 05:41:39 2026 GMT
  host: www.withshepherd.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Withshepherd Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shepherd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shepherd
provider_slug: withshepherd-com
slug: withshepherd-com-domain-security
source_filename: withshepherd-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.withshepherd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 05:41:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: withshepherd.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/withshepherd-com/security/withshepherd-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Construction
- Renewable Energy
- Technology
---
