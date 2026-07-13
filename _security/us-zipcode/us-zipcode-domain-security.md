---
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smarty.com
  spf: true
hosts:
- cert_expires: Sep 14 04:52:55 2026 GMT
  host: www.smarty.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Zipcode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US ZipCode, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: US ZipCode
provider_slug: us-zipcode
slug: us-zipcode-domain-security
source_filename: us-zipcode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smarty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:52:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: smarty.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-zipcode/refs/heads/main/security/us-zipcode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Geocoding
- Public APIs
---
