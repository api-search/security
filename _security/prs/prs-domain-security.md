---
description: ''
domains:
- caa:
  - 0 issue "symantec.com"
  - 0 iodef "mailto:servernetworks@prsformusic.com"
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: prsformusic.com
  spf: true
hosts:
- cert_expires: Jan 21 15:38:11 2027 GMT
  host: prsformusic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Prs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PRS for Music, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PRS for Music
provider_slug: prs
slug: prs-domain-security
source_filename: prs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prsformusic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 15:38:11 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: prsformusic.com\n  dnssec: false\n  caa:\n  - 0 issue \"symantec.com\"\n  - 0 iodef \"mailto:servernetworks@prsformusic.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prs/refs/heads/main/security/prs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Music
- Royalties
- Licensing
- Rights
---
