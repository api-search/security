---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: connectedcars.io
  spf: true
hosts:
- cert_expires: Jan 19 22:43:27 2027 GMT
  host: connectedcars.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Connectedcars Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connected Cars, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Connected Cars
provider_slug: connectedcars-io
slug: connectedcars-io-domain-security
source_filename: connectedcars-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: connectedcars.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 22:43:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: connectedcars.io\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/connectedcars-io/security/connectedcars-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Connected Car Platform
- Real-time Vehicle Data
- OEM APIs
- Dealers
- Importers
- Automotive Data
- Predictive Analytics
- Workshop Solutions
---
