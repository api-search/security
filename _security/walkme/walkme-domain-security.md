---
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: walkme.com
  spf: true
hosts:
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: www.walkme.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developers.walkme.com
  https: false
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: api.walkme.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Walkme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WalkMe, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WalkMe
provider_slug: walkme
slug: walkme-domain-security
source_filename: walkme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.walkme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: false\n- host: developers.walkme.com\n  https: false\n- host: api.walkme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: walkme.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/walkme/refs/heads/main/security/walkme-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Digital Adoption
- In-App Guidance
- Productivity
- Analytics
- Onboarding
---
