---
api_specs:
- filename: nuclei-openapi.yml
  format: yaml
  label: Nuclei
  slug: nuclei
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclei/refs/heads/main/openapi/nuclei-openapi.yml
- filename: nuclei-openapi.yml
  format: yaml
  label: ProjectDiscovery Cloud Platform API
  slug: projectdiscovery-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclei/refs/heads/main/openapi/nuclei-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: projectdiscovery.io
  spf: true
hosts:
- cert_expires: Aug 20 13:26:43 2026 GMT
  host: nuclei.projectdiscovery.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 13:53:51 2026 GMT
  host: docs.projectdiscovery.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:22:58 2026 GMT
  host: api.projectdiscovery.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nuclei Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nuclei, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Nuclei
provider_slug: nuclei
slug: nuclei-domain-security
source_filename: nuclei-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nuclei.projectdiscovery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 13:26:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.projectdiscovery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 13:53:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.projectdiscovery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:22:58 2026 GMT\n  hsts: null\ndomains:\n- domain: projectdiscovery.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuclei/refs/heads/main/security/nuclei-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security Testing
- Testing
- Vulnerability Scanner
- DAST
- Open Source
---
