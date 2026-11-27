---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gitshow.dev
  spf: false
hosts:
- cert_expires: Dec 25 15:16:13 2026 GMT
  host: gitshow.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GitShow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GitShow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: GitShow
provider_slug: gitshow-dev
slug: gitshow-dev-domain-security
source_filename: gitshow-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gitshow.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 15:16:13 2026 GMT\n  hsts: false\ndomains:\n- domain: gitshow.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/gitshow-dev/security/gitshow-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Developer Tools
- Open Source
- Portfolio
- GitHub
- Free
---
