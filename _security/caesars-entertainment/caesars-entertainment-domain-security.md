---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: caesars.com
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: www.caesars.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caesars Entertainment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caesars Entertainment, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Caesars Entertainment
provider_slug: caesars-entertainment
slug: caesars-entertainment-domain-security
source_filename: caesars-entertainment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caesars.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: caesars.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caesars-entertainment/refs/heads/main/security/caesars-entertainment-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Hospitality
- Gaming
- Casino
- Resorts
- Entertainment
- Loyalty
- Company
- Fortune 500
---
