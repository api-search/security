---
api_specs:
- filename: applied-industrial-technologies-orders-api-openapi.yml
  format: yaml
  label: Applied Industrial Technologies Orders API
  slug: applied-industrial-technologies-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applied-industrial-technologies/refs/heads/main/openapi/applied-industrial-technologies-orders-api-openapi.yml
- filename: applied-industrial-technologies-products-api-openapi.yml
  format: yaml
  label: Applied Industrial Technologies Products API
  slug: applied-industrial-technologies-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applied-industrial-technologies/refs/heads/main/openapi/applied-industrial-technologies-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: applied.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: applied-industrial-technologies.com
  spf: false
hosts:
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: www.applied.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.applied-industrial-technologies.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Applied Industrial Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Applied Industrial Technologies, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Applied Industrial Technologies
provider_slug: applied-industrial-technologies
slug: applied-industrial-technologies-domain-security
source_filename: applied-industrial-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.applied.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: null\n- host: api.applied-industrial-technologies.com\n  https: false\ndomains:\n- domain: applied.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: applied-industrial-technologies.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/applied-industrial-technologies/refs/heads/main/security/applied-industrial-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Industrial Distribution
- Bearings
- Power Transmission
- Fluid Power
- Supply Chain
- Fortune 1000
---
