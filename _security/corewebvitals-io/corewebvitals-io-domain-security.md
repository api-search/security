---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: corewebvitals.io
  spf: true
hosts:
- cert_expires: Dec 21 04:45:51 2026 GMT
  host: corewebvitals.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CoreWebVitals.io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoreWebVitals.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CoreWebVitals.io
provider_slug: corewebvitals-io
slug: corewebvitals-io-domain-security
source_filename: corewebvitals-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corewebvitals.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 04:45:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: corewebvitals.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/corewebvitals-io/security/corewebvitals-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Core Web Vitals
- Web Performance
- Page Speed
- Real User Monitoring
- Consulting
- MCP
---
