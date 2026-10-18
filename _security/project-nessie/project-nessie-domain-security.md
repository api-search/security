---
api_specs:
- filename: project-nessie-config-api-openapi.yml
  format: yaml
  label: Project Nessie Config API
  slug: project-nessie-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/project-nessie/refs/heads/main/openapi/project-nessie-config-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: projectnessie.org
  spf: true
hosts:
- cert_expires: Nov 21 05:21:21 2026 GMT
  host: projectnessie.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Project Nessie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Project Nessie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Project Nessie
provider_slug: project-nessie
slug: project-nessie-domain-security
source_filename: project-nessie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: projectnessie.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 05:21:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: projectnessie.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/project-nessie/refs/heads/main/security/project-nessie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Open Source
- DataLake
- Version Control
- Community
---
