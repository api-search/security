---
api_specs:
- filename: mparticle-data-plan-api-openapi.yml
  format: yaml
  label: mParticle Data Plan API
  slug: mparticle-data-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-data-plan-api-openapi.yml
- filename: mparticle-data-plan-version-api-openapi.yml
  format: yaml
  label: mParticle Data Plan Version API
  slug: mparticle-data-plan-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-data-plan-version-api-openapi.yml
- filename: mparticle-events-api-openapi.yml
  format: yaml
  label: mParticle Events API
  slug: mparticle-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-events-api-openapi.yml
- filename: mparticle-identify-api-openapi.yml
  format: yaml
  label: mParticle Identify API
  slug: mparticle-identify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-identify-api-openapi.yml
- filename: mparticle-login-api-openapi.yml
  format: yaml
  label: mParticle Login API
  slug: mparticle-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-login-api-openapi.yml
- filename: mparticle-logout-api-openapi.yml
  format: yaml
  label: mParticle Logout API
  slug: mparticle-logout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-logout-api-openapi.yml
- filename: mparticle-modify-api-openapi.yml
  format: yaml
  label: mParticle Modify API
  slug: mparticle-modify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-modify-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@mparticle.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mparticle.com
  spf: true
hosts:
- cert_expires: Oct 28 10:00:01 2026 GMT
  host: www.mparticle.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 16:14:54 2026 GMT
  host: docs.mparticle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 16:14:54 2026 GMT
  host: s2s.mparticle.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mparticle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mParticle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: mParticle
provider_slug: mparticle
slug: mparticle-domain-security
source_filename: mparticle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mparticle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 10:00:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.mparticle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:14:54 2026 GMT\n  hsts: false\n- host: s2s.mparticle.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 16:14:54 2026 GMT\n  hsts: null\ndomains:\n- domain: mparticle.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@mparticle.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/security/mparticle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Data Platform
- CDP
- Analytics
- Identity Resolution
- Audience
- Data Pipeline
- Marketing Data
- Event Streaming
- Data Governance
---
