---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:junaid.baig@leucinetech.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leucine.io
  spf: true
  spf_record: include:3978454.spf05.hubspotemail.net
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leucine.ai
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:3978454.spf05.hubspotemail.net include:amazonses.com include:servers.mcsv.net ~all
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:junaid.baig@leucinetech.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: leucinetech.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:3978454.spf05.hubspotemail.net -all
hosts:
- cert_expires: Sep 29 00:02:42 2026 GMT
  host: www.leucine.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 20:58:44 2026 GMT
  host: support.leucine.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 10:45:52 2026 GMT
  host: leucine.ai
  hsts: false
  https: true
  note: Cloudflare returns 403 to non-browser user agents; HSTS header not observed
  tls_version: TLSv1.3
- cert_expires: Aug 25 12:12:35 2026 GMT
  host: leucinetech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leucine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leucine, probed live across 4 host(s) and 3 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Leucine
provider_slug: leucine
slug: leucine-domain-security
source_filename: leucine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (no OpenAPI hosts — Leucine publishes\n  no public API)\nnotes: Leucine operates three domains mid-migration — leucinetech.com (legacy, 301s\n  to www.leucine.io), leucine.io (primary content host), and leucine.ai (migration\n  target, Cloudflare-fronted and 403 to non-browser clients).\nhosts:\n- host: www.leucine.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 00:02:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.leucine.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 20:58:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: leucine.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 10:45:52 2026 GMT\n  hsts: false\n  note: Cloudflare returns 403 to non-browser user agents; HSTS header not observed\n- host: leucinetech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 12:12:35 2026 GMT\n\
  \  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: leucine.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:junaid.baig@leucinetech.com\"\n  spf: true\n  spf_record: include:3978454.spf05.hubspotemail.net\n  dmarc: true\n  dmarc_policy: none\n- domain: leucine.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:3978454.spf05.hubspotemail.net\n    include:amazonses.com include:servers.mcsv.net ~all\n  dmarc: true\n  dmarc_policy: none\n- domain: leucinetech.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:junaid.baig@leucinetech.com\"\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:3978454.spf05.hubspotemail.net\n    -all\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leucine/refs/heads/main/security/leucine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Pharmaceutical
- Manufacturing
- Quality Management
- Life Sciences
- Regulatory Compliance
- Artificial Intelligence
- Manufacturing Execution System
- Laboratory
---
