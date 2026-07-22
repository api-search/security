---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: newoldstamp.com
  spf: true
hosts:
- cert_expires: Sep  5 07:23:19 2026 GMT
  host: newoldstamp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Newoldstamp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Newoldstamp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Newoldstamp
provider_slug: newoldstamp
slug: newoldstamp-domain-security
source_filename: newoldstamp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: newoldstamp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 07:23:19 2026 GMT\n  hsts: false\ndomains:\n- domain: newoldstamp.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newoldstamp/refs/heads/main/security/newoldstamp-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Email Signatures
- Email Signature Management
- Email Marketing
- Branding
- SaaS
- Productivity
- Website Visitor Identification
---
