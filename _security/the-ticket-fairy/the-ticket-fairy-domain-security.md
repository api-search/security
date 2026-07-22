---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ticketfairy.com
  spf: true
hosts:
- cert_expires: Oct 10 20:33:58 2026 GMT
  host: ticketfairy.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Ticket Fairy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Ticket Fairy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: The Ticket Fairy
provider_slug: the-ticket-fairy
slug: the-ticket-fairy-domain-security
source_filename: the-ticket-fairy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ticketfairy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 20:33:58 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ticketfairy.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-ticket-fairy/refs/heads/main/security/the-ticket-fairy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ticketing
- Events
- Event Management
- Payments
- Marketing
- Entertainment
---
