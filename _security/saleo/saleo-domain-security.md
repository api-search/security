---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: saleo.io
  spf: true
hosts:
- cert_expires: Oct  3 14:51:44 2026 GMT
  host: www.saleo.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: app.platform.saleo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: help.saleo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: api.platform.saleo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Added by hand — the SCIM API host is the 4th host on this provider and fell outside the probe script's max_hosts window. Observed 2026-08-13 on https://api.platform.saleo.io/scim/v2/Users (HTTP 401, HTTP/2, TLS verify ok).
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Saleo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saleo, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Saleo
provider_slug: saleo
slug: saleo-domain-security
source_filename: saleo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saleo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:51:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.platform.saleo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.saleo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.platform.saleo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: 'Added by hand — the SCIM API host is the 4th host on this provider and fell\n    outside the probe script''s max_hosts window. Observed 2026-08-13 on\n    https://api.platform.saleo.io/scim/v2/Users (HTTP 401, HTTP/2, TLS verify ok).'\ndomains:\n- domain: saleo.io\n  dnssec: true\n\
  \  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saleo/refs/heads/main/security/saleo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Sales Tech
- Demo Automation
- Sales Enablement
- Presales
- Go-To-Market
- AI Agents
- SCIM
- Identity Provisioning
- Single Sign-On
- Interactive Demos
- Product Tours
---
