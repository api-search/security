---
api_specs:
- filename: skyhigh-tenant-api-openapi.yml
  format: yaml
  label: Skyhigh Security Tenant API
  slug: skyhigh-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyhigh/refs/heads/main/openapi/skyhigh-tenant-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: skyhighsecurity.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: myshn.net
  spf: false
hosts:
- cert_expires: Dec 22 12:01:45 2026 GMT
  host: www.skyhighsecurity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 03:53:57 2026 GMT
  host: success.skyhighsecurity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 21:16:27 2027 GMT
  host: www.myshn.net
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Skyhigh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skyhigh Security, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Skyhigh Security
provider_slug: skyhigh
slug: skyhigh-domain-security
source_filename: skyhigh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.skyhighsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 12:01:45 2026 GMT\n  hsts: false\n- host: success.skyhighsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 03:53:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.myshn.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 21:16:27 2027 GMT\n  hsts: true\n  hsts_max_age: 315360000\ndomains:\n- domain: skyhighsecurity.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: myshn.net\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skyhigh/refs/heads/main/security/skyhigh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Security Service Edge
- CASB
- Secure Web Gateway
- Data Loss Prevention
- Cloud Security
- Zero Trust
- SASE
---
