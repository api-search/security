---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: every.org
  spf: true
hosts:
- cert_expires: Oct  8 09:33:01 2026 GMT
  host: www.every.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 01:54:29 2026 GMT
  host: partners.every.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Every Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Every.org, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Every.org
provider_slug: every-org
slug: every-org-domain-security
source_filename: every-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.every.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 09:33:01 2026 GMT\n  hsts: null\n- host: partners.every.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 01:54:29 2026 GMT\n  hsts: null\ndomains:\n- domain: every.org\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/every-org/refs/heads/main/security/every-org-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Charities
- Donations
- Fundraising
---
