---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:domains@fandom.com"
  - 0 iodef "mailto:ops-l@fandom.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fandom.com
  spf: true
hosts:
- cert_expires: Oct 13 12:56:52 2026 GMT
  host: www.fandom.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 17:31:30 2026 GMT
  host: community.fandom.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fandom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fandom, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fandom
provider_slug: fandom
slug: fandom-domain-security
source_filename: fandom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fandom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 12:56:52 2026 GMT\n  hsts: null\n- host: community.fandom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 17:31:30 2026 GMT\n  hsts: null\ndomains:\n- domain: fandom.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:domains@fandom.com\"\n  - 0 iodef \"mailto:ops-l@fandom.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fandom/refs/heads/main/security/fandom-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Wiki
- MediaWiki
- Media
- Entertainment
- Community
- Content
- Fan Community
---
