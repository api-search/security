---
api_specs:
- filename: sigma-aldrich-product-openapi.yml
  format: yaml
  label: Sigma-Aldrich Product Search API
  slug: sigma-aldrich-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sigma-aldrich/refs/heads/main/openapi/sigma-aldrich-product-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sigmaaldrich.com
  spf: true
hosts:
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: www.sigmaaldrich.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: api.sigmaaldrich.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sigma Aldrich Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sigma-Aldrich, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sigma-Aldrich
provider_slug: sigma-aldrich
slug: sigma-aldrich-domain-security
source_filename: sigma-aldrich-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sigmaaldrich.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: null\n- host: api.sigmaaldrich.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sigmaaldrich.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sigma-aldrich/refs/heads/main/security/sigma-aldrich-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Life Science
- Chemistry
- Biochemistry
- Laboratory
- Research
- Chemical Catalog
---
