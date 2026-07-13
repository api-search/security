---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:tls-abuse@cloudflare.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cloudflare.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zscaler.com
  spf: true
hosts:
- cert_expires: Oct  4 07:46:56 2026 GMT
  host: www.cloudflare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: www.zscaler.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 20:36:02 2026 GMT
  host: www.netskope.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zero Trust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zero Trust, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Zero Trust
provider_slug: zero-trust
slug: zero-trust-domain-security
source_filename: zero-trust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:46:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.zscaler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.netskope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 20:36:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloudflare.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:tls-abuse@cloudflare.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zscaler.com\n  dnssec: false\n  caa:\n  - 0 issue\
  \ \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zero-trust/refs/heads/main/security/zero-trust-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Access Control
- Cloud Security
- Cybersecurity
- Federal
- Identity and Access Management
- Network Security
- Security
- Zero Trust
---
