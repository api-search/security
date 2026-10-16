---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:abuse@svk.se"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: svk.se
  spf: true
hosts:
- cert_expires: Dec 30 22:45:05 2026 GMT
  host: svk.se
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Svenska Kraftnat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Svenska kraftnät, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Svenska kraftnät
provider_slug: svenska-kraftnat
slug: svenska-kraftnat-domain-security
source_filename: svenska-kraftnat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: svk.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 22:45:05 2026 GMT\n  hsts: false\ndomains:\n- domain: svk.se\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:abuse@svk.se\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/svenska-kraftnat/refs/heads/main/security/svenska-kraftnat-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Energy
- Transmission
- Grid
- Sweden
- Utilities
- Company
---
