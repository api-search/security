---
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
  dnssec: true
  domain: cloudflare.com
  spf: true
hosts:
- cert_expires: Oct  4 07:46:56 2026 GMT
  host: www.cloudflare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 16:43:14 2026 GMT
  host: developers.cloudflare.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:15:42 2026 GMT
  host: api.cloudflare.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudflare Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloudflare.com, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cloudflare.com
provider_slug: cloudflare-com
slug: cloudflare-com-domain-security
source_filename: cloudflare-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:46:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.cloudflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 16:43:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.cloudflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:15:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cloudflare.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudflare-com/refs/heads/main/security/cloudflare-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Alias
- Application Services
- CDN
- DNS
- Edge Computing
- Email
- Network
- Security
- Workers
- Zero Trust
---
