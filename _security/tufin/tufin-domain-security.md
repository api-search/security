---
api_specs:
- filename: tufin-securetrack-openapi.yml
  format: yaml
  label: Tufin SecureTrack API
  slug: tufin-securetrack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-securetrack-openapi.yml
- filename: tufin-securechange-openapi.yml
  format: yaml
  label: Tufin SecureChange API
  slug: tufin-securechange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-securechange-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tufin.com
  spf: true
hosts:
- cert_expires: Jul 13 23:59:59 2026 GMT
  host: forum.tufin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 08:30:26 2026 GMT
  host: www.tufin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tufin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tufin, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tufin
provider_slug: tufin
slug: tufin-domain-security
source_filename: tufin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forum.tufin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.tufin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:30:26 2026 GMT\n  hsts: false\ndomains:\n- domain: tufin.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/security/tufin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Security
- Compliance
- Firewall Management
- Network Security
- Network Topology
- Policy Orchestration
- Risk Management
- Security Policy Management
- Zero Trust
---
