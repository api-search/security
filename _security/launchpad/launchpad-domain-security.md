---
description: ''
domains:
- caa:
  - 0 iodef "mailto:is-admin@canonical.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "letsencrypt.org; accounturi=https://acme-v01.api.letsencrypt.org/acme/reg/32541290"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: launchpad.net
  spf: true
hosts:
- cert_expires: Dec  3 10:14:32 2026 GMT
  host: launchpad.net
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Launchpad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Launchpad, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Launchpad
provider_slug: launchpad
slug: launchpad-domain-security
source_filename: launchpad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: launchpad.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 10:14:32 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: launchpad.net\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:is-admin@canonical.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org; accounturi=https://acme-v01.api.letsencrypt.org/acme/reg/32541290\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/launchpad/refs/heads/main/security/launchpad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Collaboration
- OpenSource
- BugTracking
- CodeHosting
---
