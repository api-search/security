---
api_specs:
- filename: api.github.com.json
  format: json
  label: Code and Review APIs
  slug: code-and-review
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:dns-admin@wikimedia.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wikipedia.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: internaldeveloperplatform.org
  spf: true
hosts:
- cert_expires: Sep  4 20:06:43 2026 GMT
  host: en.wikipedia.org
  hsts: true
  hsts_max_age: 106384710
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 14:02:55 2026 GMT
  host: internaldeveloperplatform.org
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Software Development Lifecycle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Software Development Lifecycle, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Software Development Lifecycle
provider_slug: software-development-lifecycle
slug: software-development-lifecycle-domain-security
source_filename: software-development-lifecycle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.wikipedia.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\n- host: internaldeveloperplatform.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 14:02:55 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: wikipedia.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:dns-admin@wikimedia.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: internaldeveloperplatform.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/software-development-lifecycle/refs/heads/main/security/software-development-lifecycle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Development Process
- Project Management
- Quality Assurance
- Software Engineering
- DevOps
- Platform Engineering
---
