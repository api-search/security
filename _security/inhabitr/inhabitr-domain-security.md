---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: inhabitr.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inhabitr.ai
  spf: true
  spf_record: v=spf1 include:dc-aa8e722993._spfm.inhabitr.ai ~all
hosts:
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: inhabitr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 05:43:48 2026 GMT
  host: inhabitr.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inhabitr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inhabitr, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Inhabitr
provider_slug: inhabitr
slug: inhabitr-domain-security
source_filename: inhabitr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the Inhabitr hosts named in apis.yml\nnote: >-\n  Two production hosts. inhabitr.com is the consumer furniture-rental storefront and\n  inhabitr.ai is the commercial-real-estate furnishing site; both are Inhabitr-operated.\n  Neither host sets Strict-Transport-Security and neither registrable domain is signed\n  with DNSSEC or publishes a CAA record. Both publish SPF and DMARC, with inhabitr.com\n  at the stricter p=reject.\nhosts:\n- host: inhabitr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: false\n- host: inhabitr.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 05:43:48 2026 GMT\n  hsts: false\ndomains:\n- domain: inhabitr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: inhabitr.ai\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:dc-aa8e722993._spfm.inhabitr.ai\
  \ ~all\n  dmarc: true\n  dmarc_policy: quarantine\nobservations:\n- id: unhandled-exception-leak\n  severity: informational\n  detail: >-\n    https://inhabitr.com/blog returns HTTP 200 carrying an unhandled PHP exception and a\n    full Slim framework stack trace, disclosing the application path /var/www/b2c and the\n    vendor dependency tree. Observed 2026-08-23. Recorded as a public-surface observation,\n    not a vulnerability report; no system was accessed and no control was defeated.\n  evidence: https://inhabitr.com/blog\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inhabitr/refs/heads/main/security/inhabitr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Furniture Rental
- Commercial Real Estate
- Property Technology
- Hospitality
- Multifamily
- Interior Design
- Procurement
- E-Commerce
- Furnishing
---
