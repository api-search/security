---
api_specs:
- filename: mparticle-openapi.yml
  format: yaml
  label: mParticle Events API
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mparticle.com
  spf: true
hosts:
- cert_expires: Aug 27 22:10:00 2026 GMT
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
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mparticle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 22:10:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.mparticle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:14:54 2026 GMT\n  hsts: false\n- host: s2s.mparticle.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 16:14:54 2026 GMT\n  hsts: null\ndomains:\n- domain: mparticle.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
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
---
