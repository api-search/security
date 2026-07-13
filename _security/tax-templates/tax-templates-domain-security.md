---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: irs.gov
  spf: true
- caa:
  - 0 iodef "mailto:Tech-PINetworkServiceOperations@intuit.com"
  - 0 issue "sectigo.com"
  - 0 issue "comodoca.com"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intuit.com
  spf: true
hosts:
- cert_expires: Aug 24 05:55:53 2026 GMT
  host: www.irs.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: developer.intuit.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: api.intuit.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tax Templates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tax Templates, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Tax Templates
provider_slug: tax-templates
slug: tax-templates-domain-security
source_filename: tax-templates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.irs.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 05:55:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.intuit.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\n- host: api.intuit.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: irs.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: intuit.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:Tech-PINetworkServiceOperations@intuit.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tax-templates/refs/heads/main/security/tax-templates-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Documentation
- Finance
- Tax
- Templates
- Compliance
---
