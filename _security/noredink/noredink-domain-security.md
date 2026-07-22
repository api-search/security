---
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: noredink.com
  spf: true
hosts:
- cert_expires: Sep  7 20:45:40 2026 GMT
  host: noredink.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noredink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NoRedInk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NoRedInk
provider_slug: noredink
slug: noredink-domain-security
source_filename: noredink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: noredink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 20:45:40 2026 GMT\n  hsts: false\ndomains:\n- domain: noredink.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noredink/refs/heads/main/security/noredink-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Education
- EdTech
- English Language Arts
- Grammar
- Writing
- Literacy
- K-12
- OAuth
- OpenID Connect
- Single Sign-On
- Rostering
- Identity
---
