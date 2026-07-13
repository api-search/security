---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openchainproject.org
  spf: true
hosts:
- cert_expires: Aug 22 12:51:05 2026 GMT
  host: www.openchainproject.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openchain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenChain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenChain
provider_slug: openchain
slug: openchain-domain-security
source_filename: openchain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openchainproject.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 12:51:05 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: openchainproject.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openchain/refs/heads/main/security/openchain-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compliance
- Licensing
- Linux Foundation
- Standards
---
