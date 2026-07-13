---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hashnode.com
  spf: true
hosts:
- cert_expires: Sep  6 08:37:51 2026 GMT
  host: hashnode.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: apidocs.hashnode.com
  https: false
- cert_expires: Sep  6 18:53:28 2026 GMT
  host: gql.hashnode.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hashnode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hashnode, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hashnode
provider_slug: hashnode
slug: hashnode-domain-security
source_filename: hashnode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hashnode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 08:37:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apidocs.hashnode.com\n  https: false\n- host: gql.hashnode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:53:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hashnode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hashnode/refs/heads/main/security/hashnode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blogging
- Developer Platform
- GraphQL
- Content Management
- Publications
- Newsletters
---
