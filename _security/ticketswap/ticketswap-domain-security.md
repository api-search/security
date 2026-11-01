---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:security@ticketswap.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ticketswap.com
  spf: true
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: ticketswap.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ticketswap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TicketSwap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TicketSwap
provider_slug: ticketswap
slug: ticketswap-domain-security
source_filename: ticketswap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ticketswap.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ticketswap.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:security@ticketswap.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ticketswap/security/ticketswap-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
---
