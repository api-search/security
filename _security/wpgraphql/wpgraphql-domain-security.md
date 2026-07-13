---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wpgraphql.com
  spf: true
hosts:
- cert_expires: Oct  4 16:58:05 2026 GMT
  host: www.wpgraphql.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wpgraphql Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WPGraphQL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WPGraphQL
provider_slug: wpgraphql
slug: wpgraphql-domain-security
source_filename: wpgraphql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wpgraphql.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 16:58:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: wpgraphql.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wpgraphql/refs/heads/main/security/wpgraphql-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GraphQL
- WordPress
- Headless CMS
- Content Management
- Open Source
- Plugin
- Decoupled WordPress
---
