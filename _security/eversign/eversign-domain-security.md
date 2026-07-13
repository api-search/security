---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eversign.com
  spf: true
hosts:
- cert_expires: Aug 22 17:18:06 2026 GMT
  host: eversign.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: api.eversign.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eversign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eversign, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Eversign
provider_slug: eversign
slug: eversign-domain-security
source_filename: eversign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eversign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 17:18:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.eversign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: eversign.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eversign/refs/heads/main/security/eversign-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Signature
- Electronic Signatures
- Document Management
- PDF
- Audit Trail
- Webhooks
- Bulk Sending
---
