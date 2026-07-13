---
api_specs:
- filename: traiana-harmony-trade-processing-openapi.yml
  format: yaml
  label: Traiana Harmony Trade Processing API
  slug: harmony-trade-processing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/openapi/traiana-harmony-trade-processing-openapi.yml
- filename: traiana-harmony-creditlink-openapi.yml
  format: yaml
  label: Traiana Harmony CreditLink API
  slug: harmony-creditlink
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/openapi/traiana-harmony-creditlink-openapi.yml
- filename: traiana-harmony-netlink-openapi.yml
  format: yaml
  label: Traiana Harmony NetLink API
  slug: harmony-netlink
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/openapi/traiana-harmony-netlink-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cmegroup.com
  spf: true
- caa:
  - 0 iodef "mailto:hosting@traiana.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: traiana.com
  spf: true
hosts:
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: www.cmegroup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.traiana.com
  https: false
kind: domain-security
layout: security
method: probed
name: Traiana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Traiana, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Traiana
provider_slug: traiana
slug: traiana-domain-security
source_filename: traiana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cmegroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: null\n- host: api.traiana.com\n  https: false\ndomains:\n- domain: cmegroup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: traiana.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:hosting@traiana.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/security/traiana-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Fintech
- Foreign Exchange
- Post-Trade Processing
- Risk Management
---
