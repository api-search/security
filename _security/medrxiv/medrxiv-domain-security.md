---
api_specs:
- filename: openapi.yml
  format: yaml
  label: medRxiv REST API
  slug: medrxiv-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medrxiv/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: medrxiv.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: biorxiv.org
  spf: true
hosts:
- cert_expires: Sep 19 19:32:53 2026 GMT
  host: www.medrxiv.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 15:58:56 2026 GMT
  host: api.medrxiv.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 20:53:32 2026 GMT
  host: api.biorxiv.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medrxiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for medRxiv, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: medRxiv
provider_slug: medrxiv
slug: medrxiv-domain-security
source_filename: medrxiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.medrxiv.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:32:53 2026 GMT\n  hsts: false\n- host: api.medrxiv.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:58:56 2026 GMT\n  hsts: false\n- host: api.biorxiv.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 20:53:32 2026 GMT\n  hsts: false\ndomains:\n- domain: medrxiv.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: biorxiv.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medrxiv/refs/heads/main/security/medrxiv-domain-security.yml
summary_line: TLSv1.3
tags:
- Health Sciences
- Preprints
- Research
- Open Access
- Medical Research
- Clinical Research
- Scientific Publications
---
