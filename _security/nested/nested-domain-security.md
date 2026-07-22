---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "comodoca.com"
  - 0 issue "comodoca.com"
  - 0 issue "amazonaws.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nested.com
  spf: true
hosts:
- cert_expires: Aug 24 02:38:22 2026 GMT
  host: www.nested.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nested Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nested, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: nested
provider_slug: nested
slug: nested-domain-security
source_filename: nested-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nested.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 02:38:22 2026 GMT\n  hsts: false\ndomains:\n- domain: nested.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nested/refs/heads/main/security/nested-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- PropTech
- Estate Agency
- Property
- United Kingdom
---
