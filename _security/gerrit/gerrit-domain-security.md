---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: gerritcodereview.com
  spf: false
hosts:
- cert_expires: Oct 25 19:43:57 2026 GMT
  host: www.gerritcodereview.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gerrit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gerrit Code Review, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Gerrit Code Review
provider_slug: gerrit
slug: gerrit-domain-security
source_filename: gerrit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gerritcodereview.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 19:43:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: gerritcodereview.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gerrit/refs/heads/main/security/gerrit-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Code Review
- Open Source
- Git
- Collaboration
- CI/CD
---
