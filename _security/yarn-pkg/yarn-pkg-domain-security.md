---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: false
  domain: yarnpkg.com
  spf: true
hosts:
- cert_expires: Aug 22 08:15:27 2026 GMT
  host: yarnpkg.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Yarn Pkg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yarn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Yarn
provider_slug: yarn-pkg
slug: yarn-pkg-domain-security
source_filename: yarn-pkg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yarnpkg.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 22 08:15:27 2026 GMT\n  hsts: false\ndomains:\n- domain: yarnpkg.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yarn-pkg/refs/heads/main/security/yarn-pkg-domain-security.yml
summary_line: TLSv1.2
tags:
- Package Manager
- JavaScript
- Node.js
- Monorepo
- Workspaces
- Plug'n'Play
- Open Source
- Berry
- Yarn 4
---
