---
description: ''
domains:
- caa:
  - 5 issue "awstrust.com"
  - 6 issue "amazonaws.com"
  - 0 issue "entrust.net"
  - 1 issue "letsencrypt.org"
  - 2 issue "digicert.com"
  - 3 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: virtusa.com
  spf: true
hosts:
- cert_expires: Sep 18 16:25:24 2026 GMT
  host: www.virtusa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Virtusa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virtusa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Virtusa
provider_slug: virtusa
slug: virtusa-domain-security
source_filename: virtusa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.virtusa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 16:25:24 2026 GMT\n  hsts: null\ndomains:\n- domain: virtusa.com\n  dnssec: true\n  caa:\n  - 5 issue \"awstrust.com\"\n  - 6 issue \"amazonaws.com\"\n  - 0 issue \"entrust.net\"\n  - 1 issue \"letsencrypt.org\"\n  - 2 issue \"digicert.com\"\n  - 3 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtusa/refs/heads/main/security/virtusa-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Digital Engineering
- IT Services
- Consulting
- Cloud
- Outsourcing
---
