---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@mangadex.org"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mangadex.org
  spf: true
hosts:
- cert_expires: Aug 27 09:49:34 2026 GMT
  host: api.mangadex.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mangadex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MangaDex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MangaDex
provider_slug: mangadex
slug: mangadex-domain-security
source_filename: mangadex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.mangadex.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 09:49:34 2026 GMT\n  hsts: null\ndomains:\n- domain: mangadex.org\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security@mangadex.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mangadex/refs/heads/main/security/mangadex-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Anime
- Public APIs
---
