---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: greymatter.io
  spf: true
hosts:
- cert_expires: Sep  2 20:13:35 2026 GMT
  host: greymatter.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Greymatter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greymatter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Greymatter
provider_slug: greymatter
slug: greymatter-domain-security
source_filename: greymatter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: greymatter.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:13:35 2026 GMT\n  hsts: false\ndomains:\n- domain: greymatter.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greymatter/refs/heads/main/security/greymatter-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Enterprise
- Kubernetes
- Networking
- Service Mesh
- Zero Trust
---
