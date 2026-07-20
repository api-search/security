---
api_specs:
- filename: sentinelone
  format: yaml
  label: SentinelOne Management API
  slug: management-api
  spec_type: Postman
  url: https://www.postman.com/api-evangelist/sentinelone/documentation/btzef0x/sentinelone
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sentinelone.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sentinelone.net
  spf: true
hosts:
- cert_expires: Sep 11 20:41:31 2026 GMT
  host: www.sentinelone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: <tenant>.sentinelone.net
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''<tenant>.se'
kind: domain-security
layout: security
method: probed
name: Sentinelone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SentinelOne, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SentinelOne
provider_slug: sentinelone
slug: sentinelone-domain-security
source_filename: sentinelone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sentinelone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:41:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: <tenant>.sentinelone.net\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''<tenant>.se'\n  hsts: null\ndomains:\n- domain: sentinelone.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: sentinelone.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentinelone/refs/heads/main/security/sentinelone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- XDR
- EDR
- Endpoint Protection
- Threat Detection
- Incident Response
- Cloud Security
- Identity Security
---
