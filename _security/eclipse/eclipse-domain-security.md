---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eclipse.org
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.eclipse.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: marketplace.eclipse.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: api.eclipse.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Eclipse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eclipse Foundation, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Eclipse Foundation
provider_slug: eclipse
slug: eclipse-domain-security
source_filename: eclipse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eclipse.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: marketplace.eclipse.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.eclipse.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eclipse.org\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eclipse/refs/heads/main/security/eclipse-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Eclipse Foundation
- Foundation
- Open Source
- Standards
---
