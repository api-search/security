---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zimbra.com
  spf: true
hosts:
- cert_expires: Aug 23 05:01:19 2026 GMT
  host: www.zimbra.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zimbra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zimbra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zimbra
provider_slug: zimbra
slug: zimbra-domain-security
source_filename: zimbra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zimbra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 05:01:19 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: zimbra.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zimbra/refs/heads/main/security/zimbra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Collaboration
- Calendar
- Messaging
- Open Source
- SOAP
- GraphQL
- Productivity
---
