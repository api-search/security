---
api_specs:
- filename: boston-bu-access-control-api-openapi.yml
  format: yaml
  label: Boston University Bu Access Control API
  slug: boston-bu-access-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boston/refs/heads/main/openapi/boston-bu-access-control-api-openapi.yml
- filename: boston-bu-alert-api-openapi.yml
  format: yaml
  label: Boston University Bu Alert API
  slug: boston-bu-alert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boston/refs/heads/main/openapi/boston-bu-alert-api-openapi.yml
- filename: boston-bu-blocks-api-openapi.yml
  format: yaml
  label: Boston University Bu Blocks API
  slug: boston-bu-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boston/refs/heads/main/openapi/boston-bu-blocks-api-openapi.yml
- filename: boston-bu-cmb2-customizations-api-openapi.yml
  format: yaml
  label: Boston University Bu Cmb2 Customizations API
  slug: boston-bu-cmb2-customizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boston/refs/heads/main/openapi/boston-bu-cmb2-customizations-api-openapi.yml
- filename: boston-bu-navigation-api-openapi.yml
  format: yaml
  label: Boston University Bu Navigation API
  slug: boston-bu-navigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boston/refs/heads/main/openapi/boston-bu-navigation-api-openapi.yml
- filename: boston-bu-prepress-api-openapi.yml
  format: yaml
  label: Boston University Bu Prepress API
  slug: boston-bu-prepress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boston/refs/heads/main/openapi/boston-bu-prepress-api-openapi.yml
- filename: boston-bu-site-manager-api-openapi.yml
  format: yaml
  label: Boston University Bu Site Manager API
  slug: boston-bu-site-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boston/refs/heads/main/openapi/boston-bu-site-manager-api-openapi.yml
- filename: boston-bu-slideshow-api-openapi.yml
  format: yaml
  label: Boston University Bu Slideshow API
  slug: boston-bu-slideshow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boston/refs/heads/main/openapi/boston-bu-slideshow-api-openapi.yml
- filename: boston-bu-tts-api-openapi.yml
  format: yaml
  label: Boston University Bu Tts API
  slug: boston-bu-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boston/refs/heads/main/openapi/boston-bu-tts-api-openapi.yml
- filename: boston-wordpress-core-api-openapi.yml
  format: yaml
  label: Boston University Wordpress Core API
  slug: boston-wordpress-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boston/refs/heads/main/openapi/boston-wordpress-core-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issue "emsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bu.edu
  spf: true
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: www.bu.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: open.bu.edu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Boston Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boston University, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Boston University
provider_slug: boston
slug: boston-domain-security
source_filename: boston-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: false\n- host: open.bu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bu.edu\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"emsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boston/refs/heads/main/security/boston-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- United States
- Massachusetts
- Private Research University
- Research
- Research Data
- Library
- Identity Federation
- Content Management
- Open Access
---
