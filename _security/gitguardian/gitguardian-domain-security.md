---
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gitguardian.com
  spf: true
hosts:
- cert_expires: Sep 10 16:03:11 2026 GMT
  host: api.gitguardian.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gitguardian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GitGuardian, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GitGuardian
provider_slug: gitguardian
slug: gitguardian-domain-security
source_filename: gitguardian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.gitguardian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 16:03:11 2026 GMT\n  hsts: false\ndomains:\n- domain: gitguardian.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitguardian/refs/heads/main/security/gitguardian-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Security
- Public APIs
---
