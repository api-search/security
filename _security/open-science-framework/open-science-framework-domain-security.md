---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: osf.io
  spf: true
hosts:
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: developer.osf.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Science Framework Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Science Framework, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Open Science Framework
provider_slug: open-science-framework
slug: open-science-framework-domain-security
source_filename: open-science-framework-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.osf.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: osf.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-science-framework/refs/heads/main/security/open-science-framework-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Science And Math
- Public APIs
---
