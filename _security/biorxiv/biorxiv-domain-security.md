---
api_specs:
- filename: openapi.yml
  format: yaml
  label: bioRxiv REST API
  slug: biorxiv-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biorxiv/refs/heads/main/openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: biorxiv.org
  spf: true
hosts:
- cert_expires: Oct  1 05:56:55 2026 GMT
  host: www.biorxiv.org
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
name: Biorxiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bioRxiv, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: bioRxiv
provider_slug: biorxiv
slug: biorxiv-domain-security
source_filename: biorxiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.biorxiv.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:56:55 2026 GMT\n  hsts: false\n- host: api.biorxiv.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 20:53:32 2026 GMT\n  hsts: false\ndomains:\n- domain: biorxiv.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biorxiv/refs/heads/main/security/biorxiv-domain-security.yml
summary_line: TLSv1.3
tags:
- Biology
- Preprints
- Research
- Open Access
- Life Sciences
- Scientific Publications
---
