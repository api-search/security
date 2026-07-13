---
api_specs:
- filename: symantec-sepm-api-openapi.yml
  format: yaml
  label: Symantec Endpoint Protection Manager API
  slug: sepm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symantec/refs/heads/main/openapi/symantec-sepm-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: broadcom.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "symantec.com"
  - 0 issue "amazon.com"
  - 0 issue "entrust.net"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: symantec.com
  spf: true
hosts:
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: www.broadcom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: techdocs.broadcom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: apidocs.securitycloud.symantec.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Symantec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Symantec, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Symantec
provider_slug: symantec
slug: symantec-domain-security
source_filename: symantec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.broadcom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: techdocs.broadcom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.securitycloud.symantec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: broadcom.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: symantec.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"symantec.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/symantec/refs/heads/main/security/symantec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Broadcom
- Cybersecurity
- DLP
- EDR
- Endpoint Protection
- Endpoint Security
- Security
- Symantec
- Fortune 500
---
