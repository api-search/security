---
api_specs:
- filename: chinese-narrative-chapter-lock-openapi.json
  format: json
  label: cultureBiz chapter-lock
  slug: culturebiz-chapter-lock
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chinese-narrative-chapter-lock/refs/heads/main/openapi/chinese-narrative-chapter-lock-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security+caafailure@render.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: onrender.com
  spf: false
hosts:
- cert_expires: Oct 22 21:54:17 2026 GMT
  host: culturebiz-xianxia-lock.onrender.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chinese Narrative Chapter Lock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chinese Narrative Chapter Lock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Chinese Narrative Chapter Lock
provider_slug: chinese-narrative-chapter-lock
slug: chinese-narrative-chapter-lock-domain-security
source_filename: chinese-narrative-chapter-lock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  The provider runs on a Render platform subdomain (culturebiz-xianxia-lock.onrender.com) and\n  owns no registrable domain of its own. The `domains:` block below (CAA, SPF, DMARC, DNSSEC)\n  therefore describes onrender.com — Render's platform domain, controlled by Render, not by\n  this provider. Only the host-level TLS row is attributable to the provider's deployment.\nhosts:\n- host: culturebiz-xianxia-lock.onrender.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 21:54:17 2026 GMT\n  hsts: null\ndomains:\n- domain: onrender.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security+caafailure@render.com\"\n  spf: false\n  dmarc: true\n\
  \  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chinese-narrative-chapter-lock/refs/heads/main/security/chinese-narrative-chapter-lock-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- localization
- translation
- NLP
- terminology-management
- CAT
- MT-preprocessing
- chinese-language
- webnovels
- publishing
- entertainment
---
