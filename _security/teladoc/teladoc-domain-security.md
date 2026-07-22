---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: teladoc.com
  spf: true
hosts:
- cert_expires: Aug  9 02:10:48 2026 GMT
  host: teladoc.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teladoc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teladoc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Teladoc
provider_slug: teladoc
slug: teladoc-domain-security
source_filename: teladoc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teladoc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 02:10:48 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: teladoc.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teladoc/refs/heads/main/security/teladoc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthtech
- Telehealth
- Telemedicine
- Virtual Care
- Healthcare
- Behavioral Health
- Webhooks
- API
---
