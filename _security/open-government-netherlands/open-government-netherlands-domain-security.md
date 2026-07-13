---
description: ''
domains:
- caa:
  - 0 iodef "mailto:systemteam@logius.nl"
  - 0 issue "quovadisglobal.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: overheid.nl
  spf: true
hosts:
- cert_expires: Sep  7 13:25:25 2026 GMT
  host: data.overheid.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government Netherlands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Netherlands, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Open Government, Netherlands
provider_slug: open-government-netherlands
slug: open-government-netherlands-domain-security
source_filename: open-government-netherlands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.overheid.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 13:25:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: overheid.nl\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:systemteam@logius.nl\"\n  - 0 issue \"quovadisglobal.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-netherlands/refs/heads/main/security/open-government-netherlands-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Public APIs
---
