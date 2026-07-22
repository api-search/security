---
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issuewild "google.com"
  - 0 issuewild "googlehosted.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:infra@fubo.tv"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fubo.tv
  spf: true
hosts:
- cert_expires: Mar 22 21:10:24 2027 GMT
  host: www.fubo.tv
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fubotv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fuboTV, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: fuboTV
provider_slug: fubotv
slug: fubotv-domain-security
source_filename: fubotv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fubo.tv\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 22 21:10:24 2027 GMT\n  hsts: false\ndomains:\n- domain: fubo.tv\n  dnssec: false\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"google.com\"\n  - 0 issuewild \"googlehosted.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:infra@fubo.tv\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fubotv/refs/heads/main/security/fubotv-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Consumer
- Streaming
- Live TV
- Sports
- Media
- Entertainment
- OTT
- Video
---
