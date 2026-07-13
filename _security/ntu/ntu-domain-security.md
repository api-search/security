---
api_specs:
- filename: ntu-drntu-data.yaml
  format: yaml
  label: DR-NTU (Data) Dataverse API
  slug: drntu-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-drntu-data.yaml
- filename: ntu-drntu-repo-rest.yaml
  format: yaml
  label: DR-NTU (Digital Repository) DSpace REST API
  slug: drntu-repo-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-drntu-repo-rest.yaml
- filename: ntu-drntu-repo-oai.yaml
  format: yaml
  label: DR-NTU (Digital Repository) OAI-PMH
  slug: drntu-repo-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-drntu-repo-oai.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ntu.edu.sg
  spf: true
hosts:
- cert_expires: Aug 31 15:04:27 2026 GMT
  host: www.ntu.edu.sg
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 03:46:22 2026 GMT
  host: libguides.ntu.edu.sg
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: researchdata.ntu.edu.sg
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ntu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nanyang Technological University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nanyang Technological University
provider_slug: ntu
slug: ntu-domain-security
source_filename: ntu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ntu.edu.sg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 15:04:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: libguides.ntu.edu.sg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 03:46:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: researchdata.ntu.edu.sg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ntu.edu.sg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/security/ntu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Singapore
- Research Data
- Open Data
- Repository
- Library
---
