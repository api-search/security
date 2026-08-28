---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: doubleoctopus.com
  spf: true
hosts:
- cert_expires: Oct 30 18:48:12 2026 GMT
  host: doubleoctopus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 14:52:14 2026 GMT
  host: support.doubleoctopus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Secret Double Octopus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Secret Double Octopus, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Secret Double Octopus
provider_slug: secret-double-octopus
slug: secret-double-octopus-domain-security
source_filename: secret-double-octopus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doubleoctopus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 18:48:12 2026 GMT\n  hsts: false\n- host: support.doubleoctopus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 14:52:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: doubleoctopus.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/secret-double-octopus/refs/heads/main/security/secret-double-octopus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Authentication
- Identity and Access Management
- Passwordless
- Multi-Factor Authentication
- Security
- FIDO2
- Zero Trust
- Enterprise
- Workforce Identity
---
