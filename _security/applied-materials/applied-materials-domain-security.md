---
api_specs:
- filename: applied-materials-equipment-api-openapi.yml
  format: yaml
  label: Applied Materials Equipment API
  slug: applied-materials-equipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applied-materials/refs/heads/main/openapi/applied-materials-equipment-api-openapi.yml
- filename: applied-materials-maintenance-api-openapi.yml
  format: yaml
  label: Applied Materials Maintenance API
  slug: applied-materials-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applied-materials/refs/heads/main/openapi/applied-materials-maintenance-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:dnsadmin@amat.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: appliedmaterials.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: applied-materials.com
  spf: false
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: www.appliedmaterials.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.applied-materials.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Applied Materials Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Applied Materials, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Applied Materials
provider_slug: applied-materials
slug: applied-materials-domain-security
source_filename: applied-materials-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.appliedmaterials.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\n- host: api.applied-materials.com\n  https: false\ndomains:\n- domain: appliedmaterials.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:dnsadmin@amat.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: applied-materials.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/applied-materials/refs/heads/main/security/applied-materials-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Semiconductors
- Manufacturing
- Equipment
- Fab Operations
- Materials Engineering
- Fortune 500
---
