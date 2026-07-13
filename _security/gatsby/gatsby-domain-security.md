---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gatsbyjs.com
  spf: true
hosts:
- cert_expires: Aug 13 01:53:50 2026 GMT
  host: www.gatsbyjs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gatsby Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gatsby, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gatsby
provider_slug: gatsby
slug: gatsby-domain-security
source_filename: gatsby-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gatsbyjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 01:53:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gatsbyjs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gatsby/refs/heads/main/security/gatsby-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Static Site Generator
- JAMstack
- React
- GraphQL
- Build Tool
- Frontend Framework
- Web Development
---
