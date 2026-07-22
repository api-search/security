---
api_specs:
- filename: projectdiscovery-openapi-original.yml
  format: yaml
  label: ProjectDiscovery Cloud Platform (PDCP) API
  slug: projectdiscovery-cloud-platform-pdcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/projectdiscovery/refs/heads/main/openapi/projectdiscovery-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: projectdiscovery.io
  spf: true
hosts:
- cert_expires: Sep  1 01:53:40 2026 GMT
  host: projectdiscovery.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:22:58 2026 GMT
  host: api.projectdiscovery.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 13:42:35 2026 GMT
  host: api.dev.projectdiscovery.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Projectdiscovery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ProjectDiscovery, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ProjectDiscovery
provider_slug: projectdiscovery
slug: projectdiscovery-domain-security
source_filename: projectdiscovery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: projectdiscovery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 01:53:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.projectdiscovery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:22:58 2026 GMT\n  hsts: null\n- host: api.dev.projectdiscovery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:42:35 2026 GMT\n  hsts: null\ndomains:\n- domain: projectdiscovery.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/projectdiscovery/refs/heads/main/security/projectdiscovery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Security
- Vulnerability Scanning
- Attack Surface Management
- Vulnerability Management
- Asset Discovery
- DevSecOps
- Nuclei
- API
---
