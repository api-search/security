---
api_specs:
- filename: remote-cache-spec
  format: yaml
  label: Turborepo Remote Cache API
  slug: turborepo-remote-cache-api
  spec_type: OpenAPI
  url: https://turborepo.dev/api/remote-cache-spec
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: turborepo.dev
  spf: false
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vercel.com
  spf: true
hosts:
- cert_expires: Sep 20 01:09:13 2026 GMT
  host: turborepo.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 08:55:49 2026 GMT
  host: api.vercel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Turborepo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Turborepo, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Turborepo
provider_slug: turborepo
slug: turborepo-domain-security
source_filename: turborepo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: turborepo.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 01:09:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vercel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 08:55:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: turborepo.dev\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n- domain: vercel.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turborepo/refs/heads/main/security/turborepo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Build System
- Monorepo
- JavaScript
- TypeScript
- Caching
- Open Source
- Rust
- Vercel
- Developer Tools
- CI/CD
---
