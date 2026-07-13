---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openmainframeproject.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: zowe.org
  spf: true
hosts:
- cert_expires: Sep  3 05:33:38 2026 GMT
  host: www.openmainframeproject.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 19:23:48 2026 GMT
  host: www.zowe.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 12:30:23 2026 GMT
  host: galasa.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Mainframe Project Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Mainframe Project, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open Mainframe Project
provider_slug: open-mainframe-project
slug: open-mainframe-project-domain-security
source_filename: open-mainframe-project-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openmainframeproject.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 05:33:38 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: www.zowe.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:23:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: galasa.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 12:30:23 2026 GMT\n  hsts: false\ndomains:\n- domain: openmainframeproject.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: zowe.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-mainframe-project/refs/heads/main/security/open-mainframe-project-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Native
- Education
- Enterprise
- IBM Z
- Linux Foundation
- Linux on Z
- Mainframe
- Open Source
- z/OS
- z/VM
---
