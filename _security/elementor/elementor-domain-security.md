---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elementor.com
  spf: true
hosts:
- cert_expires: Sep 29 10:59:42 2026 GMT
  host: elementor.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elementor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elementor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Elementor
provider_slug: elementor
slug: elementor-domain-security
source_filename: elementor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elementor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:59:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: elementor.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elementor/refs/heads/main/security/elementor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Website Builder
- WordPress
- Page Builder
- No Code
- Web Design
- CMS
- Developer Tools
- Widgets
- Extensibility
---
