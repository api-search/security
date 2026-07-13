---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: privacy.com
  spf: true
hosts:
- cert_expires: Sep 17 17:32:22 2026 GMT
  host: privacy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Privacy Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Privacy.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Privacy.com
provider_slug: privacy-com
slug: privacy-com-domain-security
source_filename: privacy-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: privacy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 17:32:22 2026 GMT\n  hsts: false\ndomains:\n- domain: privacy.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/privacy-com/refs/heads/main/security/privacy-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Security
- Public APIs
---
