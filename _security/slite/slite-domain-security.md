---
api_specs:
- filename: openapi.json
  format: json
  label: Slite API
  slug: slite-api
  spec_type: OpenAPI
  url: https://api.slite.com/openapi.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: slite.com
  spf: true
hosts:
- cert_expires: Aug 20 07:49:53 2026 GMT
  host: developers.slite.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 16:08:00 2026 GMT
  host: api.slite.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Slite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Slite, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Slite
provider_slug: slite
slug: slite-domain-security
source_filename: slite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.slite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 07:49:53 2026 GMT\n  hsts: null\n- host: api.slite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 16:08:00 2026 GMT\n  hsts: null\ndomains:\n- domain: slite.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slite/refs/heads/main/security/slite-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Documentation
- Knowledge Base
- Collaboration
- Notes
- Team
- Asynchronous Work
- AI
- Search
---
