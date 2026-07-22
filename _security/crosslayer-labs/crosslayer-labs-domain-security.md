---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crosslayerlabs.com
  spf: true
hosts:
- cert_expires: Sep  9 17:27:40 2026 GMT
  host: www.crosslayerlabs.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crosslayer Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crosslayer Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Crosslayer Labs
provider_slug: crosslayer-labs
slug: crosslayer-labs-domain-security
source_filename: crosslayer-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crosslayerlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 17:27:40 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: crosslayerlabs.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crosslayer-labs/refs/heads/main/security/crosslayer-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Network Security
- Web Infrastructure
- Certificate Authority
- PKI
- Threat Detection
- Attack Surface
- API Security
- Cybersecurity
---
