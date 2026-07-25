---
api_specs:
- filename: prosci-adkar-assessments-api-openapi.yml
  format: yaml
  label: Prosci ADKAR Assessments API
  slug: prosci-adkar-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-adkar-assessments-api-openapi.yml
- filename: prosci-change-plans-api-openapi.yml
  format: yaml
  label: Prosci Change Plans API
  slug: prosci-change-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-change-plans-api-openapi.yml
- filename: prosci-organizations-api-openapi.yml
  format: yaml
  label: Prosci Organizations API
  slug: prosci-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-organizations-api-openapi.yml
- filename: prosci-pct-assessments-api-openapi.yml
  format: yaml
  label: Prosci PCT Assessments API
  slug: prosci-pct-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-pct-assessments-api-openapi.yml
- filename: prosci-projects-api-openapi.yml
  format: yaml
  label: Prosci Projects API
  slug: prosci-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-projects-api-openapi.yml
- filename: prosci-risk-assessment-api-openapi.yml
  format: yaml
  label: Prosci Risk Assessment API
  slug: prosci-risk-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-risk-assessment-api-openapi.yml
- filename: prosci-stakeholders-api-openapi.yml
  format: yaml
  label: Prosci Stakeholders API
  slug: prosci-stakeholders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-stakeholders-api-openapi.yml
- filename: prosci-training-api-openapi.yml
  format: yaml
  label: Prosci Training API
  slug: prosci-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-training-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prosci.com
  spf: true
hosts:
- cert_expires: Aug 25 09:57:58 2026 GMT
  host: www.prosci.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.prosci.com
  https: false
kind: domain-security
layout: security
method: probed
name: Prosci Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prosci, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Prosci
provider_slug: prosci
slug: prosci-domain-security
source_filename: prosci-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prosci.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 09:57:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.prosci.com\n  https: false\ndomains:\n- domain: prosci.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/security/prosci-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Change Management
- Methodology
- Training
---
