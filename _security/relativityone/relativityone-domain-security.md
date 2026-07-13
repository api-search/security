---
api_specs:
- filename: relativityone-legal-hold-openapi.yml
  format: yaml
  label: Legal Hold API
  slug: legal-hold-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativityone/refs/heads/main/openapi/relativityone-legal-hold-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "stratossl.digitalcertvalidation.com"
  - 0 issuewild "thawte.com"
  - 0 issuewild "volusion.digitalcertvalidation.com"
  - 0 issuewild "www.digicert.com"
  - 0 issue "1and1.digitalcertvalidation.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: relativity.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: relativity.rest
  spf: false
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: www.relativity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: platform.relativity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: relativity.rest
  https: false
kind: domain-security
layout: security
method: probed
name: Relativityone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RelativityOne, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RelativityOne
provider_slug: relativityone
slug: relativityone-domain-security
source_filename: relativityone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.relativity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.relativity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: relativity.rest\n  https: false\ndomains:\n- domain: relativity.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"stratossl.digitalcertvalidation.com\"\n  - 0 issuewild \"thawte.com\"\n  - 0 issuewild \"volusion.digitalcertvalidation.com\"\n  - 0 issuewild \"www.digicert.com\"\n  - 0 issue \"1and1.digitalcertvalidation.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: relativity.rest\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relativityone/refs/heads/main/security/relativityone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eDiscovery
- Legal
- Legal Hold
- Document Management
- Compliance
- Litigation
---
