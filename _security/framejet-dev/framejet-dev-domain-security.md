---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: framejet.dev
  spf: true
hosts:
- cert_expires: Dec  3 14:54:56 2026 GMT
  host: framejet.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Framejet Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for framejet-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: framejet-dev
provider_slug: framejet-dev
slug: framejet-dev-domain-security
source_filename: framejet-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: framejet.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 14:54:56 2026 GMT\n  hsts: null\ndomains:\n- domain: framejet.dev\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/framejet-dev/security/framejet-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Video
- API
- DeveloperTools
- Personalization
- Streaming
---
