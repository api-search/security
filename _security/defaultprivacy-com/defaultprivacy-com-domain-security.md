---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: defaultprivacy.com
  spf: true
hosts:
- cert_expires: Dec 20 10:20:07 2026 GMT
  host: defaultprivacy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Default Privacy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Default Privacy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Default Privacy
provider_slug: defaultprivacy-com
slug: defaultprivacy-com-domain-security
source_filename: defaultprivacy-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: defaultprivacy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 10:20:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: defaultprivacy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/defaultprivacy-com/security/defaultprivacy-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Directory
- Privacy Tools
- Guides
- Stacks
- Open Source
---
