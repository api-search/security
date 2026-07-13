---
api_specs:
- filename: openprovider-openapi.json
  format: json
  label: Openprovider API
  slug: openprovider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openprovider/refs/heads/main/openapi/openprovider-openapi.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: openprovider.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openprovider.eu
  spf: true
hosts:
- cert_expires: Sep 15 02:54:27 2026 GMT
  host: www.openprovider.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 08:32:52 2026 GMT
  host: docs.openprovider.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: api.openprovider.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openprovider Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Openprovider, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Openprovider
provider_slug: openprovider
slug: openprovider-domain-security
source_filename: openprovider-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openprovider.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:54:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.openprovider.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 10 08:32:52 2026 GMT\n  hsts: false\n- host: api.openprovider.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openprovider.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: openprovider.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openprovider/refs/heads/main/security/openprovider-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Domains
- DNS
- Hosting
- Reseller
- SSL Certificates
- TLDs
---
