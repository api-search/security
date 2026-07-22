---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elemy.com
  spf: true
hosts:
- cert_expires: Oct  7 00:08:38 2026 GMT
  host: care.elemy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Care Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Care, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Care
provider_slug: care
slug: care-domain-security
source_filename: care-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: care.elemy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 00:08:38 2026 GMT\n  hsts: null\ndomains:\n- domain: elemy.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/care/refs/heads/main/security/care-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
