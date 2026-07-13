---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: helixops.ai
  spf: true
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: netreo.com
  spf: true
hosts:
- cert_expires: Oct  8 04:58:33 2026 GMT
  host: www.helixops.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: solutions.netreo.com
  https: false
kind: domain-security
layout: security
method: probed
name: Netreo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netreo, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Netreo
provider_slug: netreo
slug: netreo-domain-security
source_filename: netreo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.helixops.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 04:58:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: solutions.netreo.com\n  https: false\ndomains:\n- domain: helixops.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: netreo.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netreo/refs/heads/main/security/netreo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Monitoring
- IT Operations
- Infrastructure Monitoring
- Network Monitoring
- Observability
---
