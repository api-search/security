---
api_specs:
- filename: caris-life-sciences-openapi.yml
  format: yaml
  label: Caris+Portal
  slug: caris-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caris-life-sciences/refs/heads/main/openapi/caris-life-sciences-openapi.yml
- filename: caris-life-sciences-openapi.yml
  format: yaml
  label: Caris EHR Integration
  slug: ehr-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caris-life-sciences/refs/heads/main/openapi/caris-life-sciences-openapi.yml
- filename: caris-life-sciences-openapi.yml
  format: yaml
  label: Caris CODEai Real-World Data
  slug: codeai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caris-life-sciences/refs/heads/main/openapi/caris-life-sciences-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: carislifesciences.com
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: caris.ai
  spf: true
hosts:
- cert_expires: Oct  7 12:06:29 2026 GMT
  host: www.carislifesciences.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 08:16:17 2026 GMT
  host: portal.caris.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caris Life Sciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caris Life Sciences, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Caris Life Sciences
provider_slug: caris-life-sciences
slug: caris-life-sciences-domain-security
source_filename: caris-life-sciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carislifesciences.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 12:06:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.caris.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 08:16:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carislifesciences.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: caris.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caris-life-sciences/refs/heads/main/security/caris-life-sciences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Precision Oncology
- Molecular Profiling
- Genomics
- Healthcare
- EHR Integration
- Real-World Data
---
