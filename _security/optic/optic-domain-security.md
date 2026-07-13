---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: useoptic.com
  spf: true
hosts:
- host: www.useoptic.com
  https: false
kind: domain-security
layout: security
method: probed
name: Optic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Optic, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Optic
provider_slug: optic
slug: optic-domain-security
source_filename: optic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.useoptic.com\n  https: false\ndomains:\n- domain: useoptic.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optic/refs/heads/main/security/optic-domain-security.yml
summary_line: DMARC
tags:
- API Governance
- Breaking Changes
- Contract Testing
- Diff
- Linting
- OpenAPI
- Testing
---
