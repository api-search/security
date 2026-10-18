---
api_specs:
- filename: skillsdirectory-com-categories-api-openapi.yml
  format: yaml
  label: Skills Directory Categories API
  slug: skillsdirectory-com-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skillsdirectory-com/refs/heads/main/openapi/skillsdirectory-com-categories-api-openapi.yml
- filename: skillsdirectory-com-registry-api-openapi.yml
  format: yaml
  label: Skills Directory Registry API
  slug: skillsdirectory-com-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skillsdirectory-com/refs/heads/main/openapi/skillsdirectory-com-registry-api-openapi.yml
- filename: skillsdirectory-com-scan-api-openapi.yml
  format: yaml
  label: Skills Directory Scan API
  slug: skillsdirectory-com-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skillsdirectory-com/refs/heads/main/openapi/skillsdirectory-com-scan-api-openapi.yml
- filename: skillsdirectory-com-skills-api-openapi.yml
  format: yaml
  label: Skills Directory Skills API
  slug: skillsdirectory-com-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skillsdirectory-com/refs/heads/main/openapi/skillsdirectory-com-skills-api-openapi.yml
- filename: skillsdirectory-com-stats-api-openapi.yml
  format: yaml
  label: Skills Directory Stats API
  slug: skillsdirectory-com-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skillsdirectory-com/refs/heads/main/openapi/skillsdirectory-com-stats-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: skillsdirectory.com
  spf: true
hosts:
- cert_expires: Nov 21 13:36:33 2026 GMT
  host: www.skillsdirectory.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Skillsdirectory Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skills Directory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Skills Directory
provider_slug: skillsdirectory-com
slug: skillsdirectory-com-domain-security
source_filename: skillsdirectory-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.skillsdirectory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 13:36:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: skillsdirectory.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skillsdirectory-com/refs/heads/main/security/skillsdirectory-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agent Skills
- AI Agents
- Claude
- Directory
- Security Scanning
---
