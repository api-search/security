---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: trussle.com
  spf: true
hosts:
- cert_expires: Oct  7 03:23:02 2026 GMT
  host: trussle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trussle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trussle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Trussle
provider_slug: trussle
slug: trussle-domain-security
source_filename: trussle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trussle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:23:02 2026 GMT\n  hsts: false\ndomains:\n- domain: trussle.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trussle/refs/heads/main/security/trussle-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Mortgage
- Fintech
- Financial Services
- United Kingdom
- Broker
- Acquired
---
