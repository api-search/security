---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: global.id
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: global.id
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Global Id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Global ID, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Global ID
provider_slug: global-id
slug: global-id-domain-security
source_filename: global-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: global.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: global.id\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/global-id/refs/heads/main/security/global-id-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Identity
- Digital Identity
- Decentralized Identity
- Self-Sovereign Identity
- Verifiable Credentials
- Authentication
- OAuth
---
