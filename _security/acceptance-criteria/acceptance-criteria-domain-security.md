---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agilealliance.org
  spf: true
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: atlassian.com
  spf: true
hosts:
- cert_expires: Aug 24 13:32:16 2026 GMT
  host: www.agilealliance.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: developer.atlassian.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: your-domain.atlassian.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acceptance Criteria Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acceptance Criteria, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Acceptance Criteria
provider_slug: acceptance-criteria
slug: acceptance-criteria-domain-security
source_filename: acceptance-criteria-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agilealliance.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 13:32:16 2026 GMT\n  hsts: false\n- host: developer.atlassian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: your-domain.atlassian.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agilealliance.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: atlassian.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  - 0 issue \"globalsign.com\"\n  spf:\
  \ true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acceptance-criteria/refs/heads/main/security/acceptance-criteria-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agile
- Behavior Driven Development
- Gherkin
- Quality Assurance
- Requirements
- Testing
- User Stories
---
