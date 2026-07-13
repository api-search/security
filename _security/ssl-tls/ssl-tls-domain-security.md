---
api_specs:
- filename: ssl-tls-certificate-management-openapi.yml
  format: yaml
  label: Let's Encrypt ACME API
  slug: lets-encrypt-acme
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ssl-tls/refs/heads/main/openapi/ssl-tls-certificate-management-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issuewild "www.digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: letsencrypt.org
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: digicert.com
  spf: true
hosts:
- cert_expires: Oct  4 15:24:33 2026 GMT
  host: letsencrypt.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 22:59:31 2026 GMT
  host: acme-v02.api.letsencrypt.org
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: www.digicert.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ssl Tls Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SSL/TLS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SSL/TLS
provider_slug: ssl-tls
slug: ssl-tls-domain-security
source_filename: ssl-tls-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: letsencrypt.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:24:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: acme-v02.api.letsencrypt.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 22:59:31 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\n- host: www.digicert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: letsencrypt.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issuewild \"www.digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: digicert.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n\
  \  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ssl-tls/refs/heads/main/security/ssl-tls-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SSL/TLS
- TLS
- Certificates
- PKI
- Cryptography
- Certificate Authority
- HTTPS
---
