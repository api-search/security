---
api_specs:
- filename: systemd1-openapi.yml
  format: yaml
  label: systemd Manager (org.freedesktop.systemd1)
  slug: org-freedesktop-systemd1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systemd/refs/heads/main/openapi/systemd1-openapi.yml
- filename: login1-openapi.yml
  format: yaml
  label: systemd-logind (org.freedesktop.login1)
  slug: org-freedesktop-login1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systemd/refs/heads/main/openapi/login1-openapi.yml
- filename: network1-openapi.yml
  format: yaml
  label: systemd-networkd (org.freedesktop.network1)
  slug: org-freedesktop-network1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systemd/refs/heads/main/openapi/network1-openapi.yml
- filename: resolve1-openapi.yml
  format: yaml
  label: systemd-resolved (org.freedesktop.resolve1)
  slug: org-freedesktop-resolve1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systemd/refs/heads/main/openapi/resolve1-openapi.yml
- filename: machine1-openapi.yml
  format: yaml
  label: systemd-machined (org.freedesktop.machine1)
  slug: org-freedesktop-machine1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systemd/refs/heads/main/openapi/machine1-openapi.yml
- filename: hostname1-openapi.yml
  format: yaml
  label: systemd-hostnamed (org.freedesktop.hostname1)
  slug: org-freedesktop-hostname1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systemd/refs/heads/main/openapi/hostname1-openapi.yml
- filename: varlink-openapi.yml
  format: yaml
  label: systemd Varlink Interfaces (io.systemd.*)
  slug: io-systemd-varlink
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systemd/refs/heads/main/openapi/varlink-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: systemd.io
  spf: false
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freedesktop.org
  spf: true
hosts:
- cert_expires: Sep 28 13:41:25 2026 GMT
  host: systemd.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 06:19:11 2026 GMT
  host: www.freedesktop.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Systemd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for systemd, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: systemd
provider_slug: systemd
slug: systemd-domain-security
source_filename: systemd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: systemd.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:41:25 2026 GMT\n  hsts: false\n- host: www.freedesktop.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 06:19:11 2026 GMT\n  hsts: false\ndomains:\n- domain: systemd.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: freedesktop.org\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/systemd/refs/heads/main/security/systemd-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Boot
- Cgroups
- Container
- D-Bus
- Init
- IPC
- Journal
- Linux
- Logging
- Network
- Open Source
- PID 1
- Service Manager
- System
- Systemd
- Varlink
---
