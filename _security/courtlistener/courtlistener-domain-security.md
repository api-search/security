---
description: ''
domains:
- caa:
  - 0 iodef "mailto:caa-violations@free.law"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: courtlistener.com
  spf: true
hosts:
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: www.courtlistener.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Courtlistener Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CourtListener, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CourtListener
provider_slug: courtlistener
slug: courtlistener-domain-security
source_filename: courtlistener-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.courtlistener.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: courtlistener.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa-violations@free.law\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/courtlistener/refs/heads/main/security/courtlistener-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Legal
- Nonprofit
- OpenData
- CourtListener
- FreeLaw
---
