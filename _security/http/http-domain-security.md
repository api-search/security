---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "awstrust.com"
  - 0 iodef "mailto:foxsec+caaiodef@mozilla.com"
  - 0 issue "sectigo.com"
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mozilla.org
  spf: true
hosts:
- cert_expires: Aug 24 14:38:53 2026 GMT
  host: developer.mozilla.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Http Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HTTP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HTTP
provider_slug: http
slug: http-domain-security
source_filename: http-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.mozilla.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 14:38:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mozilla.org\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"awstrust.com\"\n  - 0 iodef \"mailto:foxsec+caaiodef@mozilla.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/http/refs/heads/main/security/http-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Networking
- Protocol
- Standards
- Web
---
