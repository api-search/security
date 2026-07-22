---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wivity.com
  spf: true
hosts:
- cert_expires: Oct 18 22:10:21 2026 GMT
  host: wivity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wivity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wivity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wivity
provider_slug: wivity
slug: wivity-domain-security
source_filename: wivity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wivity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 22:10:21 2026 GMT\n  hsts: false\ndomains:\n- domain: wivity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wivity/refs/heads/main/security/wivity-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Web3
- Governance
- Blockchain
- DAO
- Consortia
- Standards
---
