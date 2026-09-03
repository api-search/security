---
api_specs:
- filename: vitagroup-hip-ehrbase-openehr.json
  format: json
  label: HIP EHRbase openEHR REST API
  slug: hip-ehrbase-openehr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/openapi/vitagroup-hip-ehrbase-openehr.json
- filename: vitagroup-hip-ehrbase-admin.json
  format: json
  label: HIP EHRbase Admin API
  slug: hip-ehrbase-admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/openapi/vitagroup-hip-ehrbase-admin.json
- filename: vitagroup-hip-ehrbase-item-tags.json
  format: json
  label: HIP EHRbase Item Tag Experimental API
  slug: hip-ehrbase-item-tags
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/openapi/vitagroup-hip-ehrbase-item-tags.json
- filename: vitagroup-hip-ehrbase-enterprise.yml
  format: yaml
  label: HIP EHRbase Enterprise API
  slug: hip-ehrbase-enterprise
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/openapi/vitagroup-hip-ehrbase-enterprise.yml
- filename: vitagroup-ehrbase-sandbox-live.json
  format: json
  label: EHRbase Sandbox (live springdoc api-docs)
  slug: ehrbase-sandbox-live
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/openapi/vitagroup-ehrbase-sandbox-live.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vitagroup.ag
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ehrbase.org
  spf: false
hosts:
- cert_expires: Oct 30 19:46:10 2026 GMT
  host: www.vitagroup.ag
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 10:11:06 2026 GMT
  host: docs.ehrbase.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 03:15:58 2026 GMT
  host: sandkiste.ehrbase.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vitagroup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for vitagroup, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: vitagroup
provider_slug: vitagroup
slug: vitagroup-domain-security
source_filename: vitagroup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vitagroup.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 19:46:10 2026 GMT\n  hsts: false\n- host: docs.ehrbase.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 10:11:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sandkiste.ehrbase.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 03:15:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vitagroup.ag\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: ehrbase.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/security/vitagroup-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Health IT
- Electronic Health Records
- openEHR
- FHIR
- Clinical Data Repository
- Interoperability
- Germany
- Open Source
---
