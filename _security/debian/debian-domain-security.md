---
api_specs:
- filename: debian-sources-api-openapi.yml
  format: yaml
  label: Debian Sources API
  slug: debian-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debian/refs/heads/main/openapi/debian-sources-api-openapi.yml
- filename: debian-bugs-api-openapi.yml
  format: yaml
  label: Debian Bugs API
  slug: debian-bugs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debian/refs/heads/main/openapi/debian-bugs-api-openapi.yml
- filename: debian-copyright-api-openapi.yml
  format: yaml
  label: Debian Copyright API
  slug: debian-copyright-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debian/refs/heads/main/openapi/debian-copyright-api-openapi.yml
- filename: debian-maintainers-api-openapi.yml
  format: yaml
  label: Debian Maintainers API
  slug: debian-maintainers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debian/refs/heads/main/openapi/debian-maintainers-api-openapi.yml
- filename: debian-patches-api-openapi.yml
  format: yaml
  label: Debian Patches API
  slug: debian-patches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debian/refs/heads/main/openapi/debian-patches-api-openapi.yml
- filename: debian-reproducibility-api-openapi.yml
  format: yaml
  label: Debian Reproducibility API
  slug: debian-reproducibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debian/refs/heads/main/openapi/debian-reproducibility-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:dsa@debian.org"
  - 128 issuewild ";"
  - 128 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/346607"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: debian.org
  spf: true
hosts:
- cert_expires: Sep  1 00:53:46 2026 GMT
  host: www.debian.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 01:00:53 2026 GMT
  host: sources.debian.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 01:06:37 2026 GMT
  host: bugs.debian.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Debian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Debian, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Debian
provider_slug: debian
slug: debian-domain-security
source_filename: debian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.debian.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 00:53:46 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: sources.debian.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:00:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: bugs.debian.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 01:06:37 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: debian.org\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:dsa@debian.org\"\n  - 128 issuewild \";\"\n  - 128 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/346607\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debian/refs/heads/main/security/debian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Bug Tracker
- Debian
- Linux
- Open-Source
- Operating System
- Package Management
- Source Code
---
